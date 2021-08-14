---
title: Programfel
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931467"
---
# <a name="application-errors"></a>Programfel

Letar du efter information om **de AADSTS-felkoder** som returneras från STS-tjänsten för Azure Active Directory-säkerhetstoken (Azure AD) ? Läs [Azure AD-autentisering och auktoriseringsfelkoder](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) för att hitta AADSTS felbeskrivningar, korrigeringar och några förslag på lösningar.

Auktoriseringsfel kan vara ett resultat av flera olika problem, varav de flesta genererar ett 401- eller 403-fel. Följande kan till exempel leda till auktoriseringsfel:

- Felaktiga [förvärvsflöden av åtkomsttoken](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Dåligt konfigurerade [behörighetsomfattningar](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Brist på [medgivande](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

För att lösa vanliga auktoriseringsfel provar du de steg nedan som bäst matchar det fel du får. Fler än en kan användas.

**401 Ej behörig: Är din token giltig?**

Kontrollera att programmet presenterar en giltig åtkomsttoken till Microsoft Graph som en del av begäran. Det här felet innebär ofta att åtkomsttoken kanske saknas i rubriken för HTTP-autentiseringsbegäran eller att token är ogiltig eller har upphört att gälla. Vi rekommenderar att du använder [Microsoft Authentication Library (MSAL) för hämtning](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) av åtkomsttoken. Det här felet kan också inträffa om du försöker använda en delegerad åtkomsttoken som tilldelas ett personligt Microsoft-konto för att få åtkomst till ett API som bara har stöd för arbets- eller skolkonton (organisationskonton).

**403 Förbjudit fel: Har du valt rätt behörighetsuppsättning?**

Kontrollera att du har begärt rätt uppsättning behörigheter baserat på Microsofts Graph-API:er dina appsamtal. Rekommenderade behörigheter med minst behörighet anges i alla avsnitt om Microsoft-Graph API-referens. Dessutom måste de behörigheterna beviljas till programmet av en användare eller administratör. Att bevilja behörigheter sker vanligtvis via en medgivandesida eller genom att bevilja behörigheter med hjälp av registreringsbladet för Azure Portal-appen. I **Inställnings-** bladet för programmet klickar du på **Obligatoriska behörigheter** och klickar sedan på **Bevilja behörigheter**.

- [Microsoft Graph-behörigheter](https://docs.microsoft.com/graph/permissions-reference) 
- [Förstå Azure AD-behörigheter och medgivande](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Förbjudit fel: Har appen skaffat en token som matchar valda behörigheter?**

Kontrollera att den typ av behörighet som begärs eller beviljats matchar den typ av åtkomsttoken som appen hämtar. Du kan begära och bevilja programbehörigheter men använda delegerade interaktiva kodflödestoken i stället för flödestoken för klientbehörigheter, eller begära och bevilja delegerade behörigheter men använda flödestoken för klientbehörigheter i stället för delegerade kodflödestoken.

- [Få åtkomst för användare och delegerade behörigheter](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – OAuth 2.0 flödet för auktoriseringskod](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få åtkomst utan användare (daemon-tjänst) och programbehörigheter](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – OAuth 2.0 flödet för klientautentiseringsuppgifter](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Förbjudit fel: Återställa lösenord**

Det finns för närvarande inga programbehörigheter för daemon-tjänst till tjänst som tillåter återställning av användarlösenord. De här API:erna stöds endast med hjälp av interaktiva delegerade kodflöden med en inloggad administratör.

- [Microsoft Graph-behörigheter](https://docs.microsoft.com/graph/permissions-reference)

**403 Förbjudit: Har användaren åtkomst och är de licensierade?**

För delegerade kodflöden utvärderar Microsoft Graph om begäran tillåts utifrån de behörigheter som tilldelats appen och de behörigheter som den inloggade användaren har. I allmänhet innebär det här felet att användaren inte är privilegierad nog att utföra begäran eller användaren inte är licensierade för data som används. Endast användare med den behörighet eller licenser som krävs kan göra begäran framgångsrikt.

**403 Förbjudit: Har du valt rätt resurs-API?**

API-tjänster som Microsoft Graph kontrollerar att aud-anspråket (målgruppen) i tokenen för mottagen åtkomst matchar det värde som förväntas för sig själv, och om inte resulterar det i felet 403 Åtkomst nekas. Ett vanligt misstag som resulterar i detta fel är att man försöker använda en token som förvärvats för Azure AD Graph API:er, Outlook API:er eller SharePoint/OneDrive-API:er för att anropa Microsoft Graph (eller tvärtom). Kontrollera att resursen (eller omfattningen) som din app förvärvar en token för matchar API:t som appen anropar.

**400 Felaktig begäran eller 403 Förbjudit: Följer användaren organisationens principer för villkorsstyrd åtkomst?**

Baserat på organisationens ca-principer kan en användare som använder Microsoft Graph-resurser via programmet uppmanas att ta del av ytterligare information som inte finns i den åtkomsttoken som appen köptes från början. I det här fallet får din app ett 400-fel med ett *interaction_required*-fel vid insamling av åtkomsttoken eller ett 403-fel med *insufficient_claims*-fel när man anropar Microsoft Graph. I båda fallen innehåller felsvaret ytterligare information som kan presenteras för auktoriseringsslutpunkten för att utmaning användaren om ytterligare information (som multifaktorautentisering eller enhetsregistrering).

- [Hantera villkorsstyrda åtkomstutmaningar med MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Utvecklarvägledning för villkorlig åtkomst i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
