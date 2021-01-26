---
title: Program fel
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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984657"
---
# <a name="application-errors"></a>Program fel

Letar du efter information om **AADSTS-felkoderna** som returneras från Azure Active Directory (Azure AD) säkerhetstokentjänst? Läs [Azure AD-autentiserings-och auktoriseringsfel](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) för att hitta AADSTS fel beskrivningar, korrigeringar och vissa föreslagna lösningar.

Auktoriseringsfel kan uppstå på grund av flera olika problem, som de flesta skapar ett 401-eller 403-fel. Följande kan till exempel ge upphov till auktoriseringsfel:

- Felaktiga [inköps flöden](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) för åtkomsttoken 
- Dåligt konfigurerade [behörighets omfattningar](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [Godkännande](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) saknas

Om du vill lösa vanliga auktoriseringsfel kan du försöka med de steg som visas nedan så att det stämmer överens med det fel du får. Fler än en kan tillkomma.

**401 ej behörigt fel: är din token giltig?**

Kontrol lera att din ansökan visar en giltig åtkomsttoken för Microsoft Graph som en del av begäran. Det här felet innebär ofta att åtkomsttoken kan saknas i huvudet HTTP unheading Request eller att token är ogiltig eller har upphört att gälla. Vi rekommenderar starkt att du använder [Microsoft-autentiseringsschemat (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) för hämtning av Access-token. Dessutom kan det här fel meddelandet visas om du försöker använda en delegerad åtkomsttoken som har tilldelats ett personligt Microsoft-konto för att få åtkomst till ett API som bara stöder arbets-eller skol konton (organisations konton).

**403 otillåtet fel: har du valt rätt uppsättning behörigheter?**

Kontrol lera att du har begärt rätt uppsättning behörigheter baserat på API-anropen för Microsoft Graph. Rekommenderade minst privilegierade behörigheter tillhandahålls i alla ämnen för Microsoft Graph API Reference. Dessa behörigheter måste dessutom beviljas av en användare eller administratör. Beviljande av behörigheter sker normalt via en medgivande sida eller genom att bevilja behörigheter med hjälp av ett program registrerings blad för Azure Portal. I **inställnings** bladet för programmet klickar du på **nödvändiga behörigheter** och sedan på **tilldela behörigheter**.

- [Microsoft Graph-behörigheter](https://docs.microsoft.com/graph/permissions-reference) 
- [Förstå Azure AD-behörigheter och medgivande](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 förbud: har appen skaffat ett token för att matcha de valda behörigheterna?**

Se till att den behörighets typ som begärs eller ges matchar den typ av åtkomsttoken som appen erhåller. Du kanske begär och beviljar program behörigheter men använder delegerade interaktiva kodnings flöde för klienter i stället för flöden för klient referenser, eller begära och bevilja delegerade behörigheter, men som använder flöden för klient referenser i stället för delegerade kodningar för kod flöden.

- [Åtkomst för användares och delegerade behörigheter](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-flödet för OAuth 2,0-Authorization](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få åtkomst utan en användare (daemon-tjänst) och program behörigheter](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0 – flödet för OAuth 2,0-klienten](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 otillåtet fel: återställer lösen ordet**

För närvarande finns det inga behörigheter för behörighets daemon för program som gör att du kan återställa lösen ord. Dessa API: er stöds bara med den interaktiva delegerade kod som flödar med en inloggad administratör.

- [Microsoft Graph-behörigheter](https://docs.microsoft.com/graph/permissions-reference)

**403 förbud: har användaren åtkomst och är de licensierade?**

För delegerade kod flöden utvärderar Microsoft Graph om begäran är tillåten baserat på de behörigheter som har tilldelats programmet och de behörigheter som den inloggade användaren har. Vanligt vis anger det här felet att användaren inte är tillräckligt hemlig för att utföra begäran eller att användaren inte är licensierad för de data som nås. Endast användare med nödvändig behörighet eller licenser kan göra så att begäran lyckas.

**403 förbud: valde du rätt resurs-API?**

API-tjänster som Microsoft Graph kontrol lera att AUD-anspråk (mål gruppen) i den mottagna åtkomst-token matchar det värde som förväntas för sig själv, och om det inte så resulterar det i ett 403-otillåtet fel. Ett vanligt misstag som resulterade i att det här felet används för att använda en token som skaffats för Azure AD Graph API: er, Outlook API: er eller SharePoint/OneDrive API för samtal till Microsoft Graph (eller vice versa). Kontrol lera att resursen (eller omfattningen) som din app hämtar ett token för matchar det API som programmet ringer upp.

**400 Felaktig begäran eller 403 förbud: ser användaren att uppfylla organisationens principer för villkorsstyrd åtkomst (CA)?**

Utifrån en organisations CERTIFIKATUTFÄRDARCERTIFIKAT kan en användare som har till gång till Microsoft Graph-resurser via ditt program anropas för ytterligare information som inte finns i Access-säkerhetstoken som appen ursprungligen skaffade. I det här fallet får din app ett 400 med *interaction_required* fel under hämtning av en åtkomsttoken eller 403 med *insufficient_claims* fel när du anropar Microsoft Graph. I båda fallen innehåller fel svaret ytterligare information som kan visas för behörighets slut punkten för att utmana användaren att få ytterligare information (som multifaktorautentisering eller enhets registrering).

- [Hantera villkorade åtkomst problem med MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Utvecklings vägledning för villkorlig åtkomst för Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
