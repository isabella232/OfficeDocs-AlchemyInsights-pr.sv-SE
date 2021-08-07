---
title: Autentiseringsproblem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019526"
---
# <a name="authentication-issues"></a>Autentiseringsproblem

**Letar du efter information om de AADSTS-felkoder som returneras från Azure Active Directory (Azure AD) säkerhetstokentjänsten (STS)?** Se [Azure AD-autentisering och auktoriseringsfelkoder](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) för att hitta AADSTS-felbeskrivningar, korrigeringar och några förslag på lösningar.

Auktoriseringsfel kan vara ett resultat av flera olika problem, varav de flesta genererar ett 401- eller 403-fel. Följande problem kan till exempel leda till auktoriseringsfel:

- Felaktiga [förvärvsflöden av åtkomsttoken](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Dåligt konfigurerade [behörighetsomfattningar](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Brist på [medgivande](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

För att lösa vanliga auktoriseringsfel kan du prova de stegen nedan som bäst matchar felet som du får. Mer än ett steg kan gälla för ett fel som du får.

**401 Ej behörig: Är din token giltig?**

Se till att din app presenterar en giltig åtkomsttoken för Microsoft Graph som en del av begäran. Det här felet innebär ofta att åtkomsttoken kanske saknas i rubriken för HTTP-autentiseringsbegäran eller att token är ogiltig eller har upphört att gälla. Vi rekommenderar starkt att du använder Microsoft Authentication Library (MSAL) för förvärv av åtkomsttoken. Det här felet kan dessutom uppstå om du försöker använda en delegerad åtkomsttoken som beviljats för ett personligt Microsoft-konto för att få åtkomst till ett API som bara stöder arbets- eller skolkonton (organisationskonton).

**403 Förbjudit fel: Har du valt rätt behörighetsuppsättning?**

Kontrollera att du har begärt rätt behörighetsuppsättning baserat på de Microsoft Graph-API:erna som din app anropar. Rekommenderade minst privilegierade behörigheter finns i alla avsnitt om Microsoft Graph API-referensmetoden. Dessutom måste de behörigheterna beviljas till programmet av en användare eller administratör. Att bevilja behörigheter sker vanligen via en medgivandesida eller användning av registreringsbladet för Azure Portal-appen. I **Inställnings-** bladet för programmet klickar du på **Obligatoriska behörigheter** och klickar sedan på **Bevilja behörigheter**. Mer information finns i:

- [Microsoft Graph-behörigheter](https://docs.microsoft.com/graph/permissions-reference) 
- [Förstå Azure AD-behörigheter och medgivande](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Förbjudit fel: Har appen skaffat en token som matchar valda behörigheter?**

Kontrollera att de behörighetstyper som begärs eller beviljas matchar den typ av åtkomsttoken som din app förvärvar. Du kanske begär och beviljar programbehörigheter, men använder delegerade interaktiva kodflödestoken i stället för flödestoken för klientautentiseringsuppgifter, eller begär och beviljar delegerade behörigheter men använder flödestoken för klientautentiseringsuppgifter i stället för delegerade kodflödestoken.

Mer information om hur du hämtar token finns i:

- [Få åtkomst för användare och delegerade behörigheter](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – OAuth 2.0 flödet för auktoriseringskod](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få åtkomst utan användare (daemon-tjänst) och programbehörigheter](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – OAuth 2.0 flödet för klientautentiseringsuppgifter](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Förbjudit fel: Återställa lösenord**

Det finns för närvarande inga programbehörigheter för daemon-tjänst till tjänst som tillåter återställning av användarlösenord. De här API:erna stöds endast med hjälp av interaktiva delegerade kodflöden med en inloggad administratör. Mer information finns i [Microsoft Graph-behörigheter](https://docs.microsoft.com/graph/permissions-reference).

**403 Förbjudit: Har användaren åtkomst och är de licensierade?**

För delegerade kodflöden utvärderar Microsoft Graph om begäran har tillåtits baserat på de behörigheter som har beviljats till appen och de behörigheter som den inloggade användaren har. I allmänhet innebär det här felet att användaren inte är privilegierad nog att utföra begäran **eller** användaren inte är licensierade för data som används. Endast användare med den behörighet eller licenser som krävs kan göra begäran framgångsrikt.

**403 Förbjudit: Har du valt rätt resurs-API?**

API-tjänster som Microsoft Graph kontrollerar att anspråket (målgrupp) för *aud* i den mottagna åtkomsttoken matchar det värde som den förväntar sig själv, och om inte, uppstår ett felmeddelande om att 403 Förbjudit. Ett vanligt misstag som resulterar i detta fel är att man försöker använda en token som förvärvats för Azure AD Graph API:er, Outlook API:er eller SharePoint/OneDrive-API:er för att anropa Microsoft Graph (eller tvärtom). Kontrollera att resursen (eller omfattningen) som din app förvärvar en token för matchar API:t som appen anropar.

**400 Felaktig begäran eller 403 Förbjudit: Följer användaren organisationens principer för villkorsstyrd åtkomst?**

Baserat på en organisations villkorsstyrda åtkomstprinciper kan en användare som använder Microsoft Graph-resurser via appen uppmanas för ytterligare information som inte finns i den åtkomsttoken som appen ursprungligen förvärvat. I det här fallet får din app ett **400-fel med ett *interaction_required***-fel vid insamling av åtkomsttoken eller ett **403-fel med *insufficient_claims***-fel när man anropar Microsoft Graph. I båda fallen innehåller felmeddelandet ytterligare information som kan visas för den auktoriserade slutpunkten för att uppmana användaren att använda ytterligare information (t.ex. multifaktorautentisering eller enhetsregistrering).

Mer information om villkorsstyrd åtkomst finns i:

- [Hantera utmaningar med villkorsstyrd åtkomst med MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Utvecklarvägledning för villkorlig åtkomst i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Support för ADAL (Azure Active Directory) och Azure AD Graph API (AAD Graph)***

- Från och med den 30 juni 2020 kommer vi inte längre att lägga till nya funktioner i Azure Active Directory Authentication Library (ADAL) och Azure AD Graph API (AAD Graph). Vi kommer att fortsätta att tillhandahålla teknisk support och säkerhetsuppdateringar men tillhandahåller inte längre funktionsuppdateringar.
- Från och med den 30 juni 2022 avslutar vi supporten för ADAL och AAD Graph och tillhandahåller inte längre teknisk support eller säkerhetsuppdateringar.
    - Appar som använder ADAL i befintliga OS-versioner kommer att fortsätta att fungera efter denna tid, men får ingen teknisk support eller säkerhetsuppdateringar.
    - Appar som använder AAD Graph efter den här tiden kanske inte längre får svar från AAD Graph-slutpunkten.

**ADAL-migrering**

Vi rekommenderar uppdatering till [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de senaste funktionerna och säkerhetsuppdateringarna. Den här rekommendationen gäller Microsofts migrering av programmen till MSAL innan tidsgränsen för support har löpt ut. Syftet med migrering av Microsoft-appar till MSAL är att säkerställa att programmen kan dra nytta av MSAL:s pågående förbättringar av säkerhet och funktioner.

- [Läs vanliga frågor och svar om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Läs mer om hur du migrerar appar per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Om du behöver hjälp med att förstå vilka av dina appar använder ADAL, rekommenderar vi att du granskar alla dina appars källkod och, om tillämpligt, nå ut till oberoende programvaruleverantörer (ISV:er) eller programleverantörer. Microsoft support kan också ge dig en lista med alla ADAL-appar som inte kommer från Microsoft i din klientorganisation.

**AAD Graph-migrering**

För program som använder AAD Graph följer du våra riktlinjer för att [migrera Azure AD Graph-appar till Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [I vår checklista för migrering får du en punkt för att komma igång](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Azure-appregistreringsportalen visar vilka program som använder AAD Graph. Vi rekommenderar att du granskar alla dina appars källkod, och om tillämpligt kan du nå ut till ISV:er eller programleverantörer. Microsoft support kan också ge dig information om all AAD Graph-användning i din klientorganisation.

 










