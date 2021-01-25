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
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974790"
---
# <a name="authentication-issues"></a>Autentiseringsproblem

**Letar du efter information om AADSTS-felkoderna som returneras från Azure Active Directory (Azure AD) säkerhetstokentjänst?** Se [felkoder i Azure AD-autentisering och-auktoriseringsfel](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) för att hitta AADSTS fel beskrivningar, korrigeringar och vissa föreslagna lösningar.

Auktoriseringsfel kan uppstå på grund av flera olika problem, som de flesta skapar ett 401-eller 403-fel. Följande problem kan till exempel leda till auktoriseringsfel:

- Felaktiga [inköps flöden](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) för åtkomsttoken 
- Dåligt konfigurerade [behörighets omfattningar](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [Godkännande](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) saknas

Om du vill lösa vanliga auktoriseringsfel kan du försöka med de steg som visas nedan som stämmer överens med det fel du får. Mer än ett steg kan tillkomma för ett fel som du får.

- **401 ej behörigt fel: är din token giltig?**

Kontrol lera att din app presenterar en giltig åtkomsttoken för Microsoft Graph som en del av begäran. Det här felet innebär ofta att åtkomsttoken kan saknas i huvudet HTTP unheading Request eller att token är ogiltig eller har upphört att gälla. Vi rekommenderar starkt att du använder Microsoft-autentiseringsschemat (MSAL) för hämtning av Access-token. Dessutom kan det här fel meddelandet visas om du försöker använda en delegerad åtkomsttoken som har tilldelats ett personligt Microsoft-konto för att få åtkomst till ett API som bara stöder arbets-eller skol konton (organisations konton).

**403 otillåtet fel: har du valt rätt uppsättning behörigheter?**

Kontrol lera att du har begärt rätt behörighets uppsättning baserat på API-anropen i Microsoft Graph. Rekommenderade behörigheter för minst-privilegie rad finns i alla ämnen för Microsoft Graph API Reference. Dessa behörigheter måste dessutom beviljas av en användare eller administratör. Beviljande av behörigheter sker normalt genom en medgivande sida eller användning av bladet registrering av Azure Portal program. I **inställnings** bladet för programmet klickar du på **nödvändiga behörigheter** och sedan på **tilldela behörigheter**. Mer information finns i:

- [Microsoft Graph-behörigheter](https://docs.microsoft.com/graph/permissions-reference) 
- [Förstå Azure AD-behörigheter och medgivande](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 förbud: har appen skaffat ett token för att matcha de valda behörigheterna?**

Kontrol lera att de typer av behörigheter som begärts eller beviljats matchar den typ av åtkomsttoken som appen erhåller. Du kanske begär och beviljar program behörigheter, men använder delegerade interaktiva kodnings flöde för klienter i stället för flöden för klient referenser, eller begär och tilldelar delegerade behörigheter, men använder flöden för klient referenser i stället för delegerade kodningar för kod flöden.

Mer information om hur du köper token finns i:

- [Åtkomst för användares och delegerade behörigheter](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-flödet för OAuth 2,0-Authorization](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Få åtkomst utan en användare (daemon-tjänst) och program behörigheter](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0 – flödet för OAuth 2,0-klienten](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 otillåtet fel: återställer lösen ordet**

För närvarande finns det inga behörigheter för behörighets daemon för program som gör att du kan återställa lösen ord. Dessa API: er stöds bara med den interaktiva delegerade kod som flödar med en inloggad administratör. Mer information finns i [behörigheter i Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 förbud: har användaren åtkomst och är de licensierade?**

För delegerade kod flöden utvärderar Microsoft Graph om begäran har godkänts baserat på de behörigheter som har tilldelats programmet och de behörigheter som den inloggade användaren har. Vanligt vis anger det här felet att användaren inte är tillräckligt hemlig för att utföra begäran **eller** att användaren inte är licensierad för de data som nås. Endast användare med nödvändig behörighet eller licenser kan göra så att begäran lyckas.

**403 förbud: valde du rätt resurs-API?**

API-tjänster som Microsoft Graph kontrol lera att *AUD* -anspråk (mål gruppen) i den mottagna åtkomsttoken stämmer överens med det värde som förväntas för sig självt, och om så inte är fallet uppstår ett 403-otillåtet fel. Ett vanligt misstag som resulterade i att det här felet används för att använda en token som skaffats för Azure AD Graph API: er, Outlook API: er eller SharePoint/OneDrive API för samtal till Microsoft Graph (eller vice versa). Kontrol lera att resursen (eller omfattningen) som din app hämtar ett token för matchar det API som programmet ringer upp.

**400 Felaktig begäran eller 403 förbud: ser användaren att uppfylla organisationens principer för villkorsstyrd åtkomst (CA)?**

Baserat på organisationens principer för villkorsstyrd åtkomst (CA) kan en användare som har till gång till Microsoft Graph-resurser via ditt program anropas för ytterligare information som inte finns i Access-token som appen ursprungligen skaffade. I det här fallet får din app ett **400 med *interaction_required*** fel under hämtning av en åtkomsttoken eller **403 med *Insufficient_claims*** fel när du anropar Microsoft Graph. I båda fallen innehåller fel svaret ytterligare information som kan visas för den godkända slut punkten för att användaren ska få ytterligare information (som multifaktorautentisering eller enhets registrering).

Mer information om villkorlig åtkomst finns i:

- [Hantera villkorade åtkomst problem med MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Utvecklings vägledning för villkorlig åtkomst för Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Slut på stöd för Azure Active Directory-autentiseringspaketet (ADAL) och Azure AD Graph API (AAD-diagram)_* _

- Från den 30 juni 2020 lägger vi inte längre till några nya funktioner i Azure Active Directory-autentiseringspaketet (ADAL) och Azure AD Graph API (AAD-diagram). Vi fortsätter att tillhandahålla tekniska support-och säkerhets uppdateringar men tillhandahåller inte längre funktions uppdateringar.
- Från och med den 30 juni 2022 kommer vi att få support för ADAL och AAD-graf och inte längre erbjuda teknisk support eller säkerhets uppdateringar.
    - Program som använder ADAL i befintliga OS-versioner fortsätter att fungera efter den här tiden men kommer inte att få teknisk support eller säkerhets uppdateringar.
    - Appar som använder AAD Graph efter den här tiden får inte längre svar från slut punkten för en AAD-graf.

_ *ADAL-migrering**

Vi rekommenderar att du uppdaterar till [Microsoft-autentiseringspaketet (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de senaste funktionerna och säkerhets uppdateringarna. Denna rekommendation är att Microsoft migrera sina program till MSAL efter tids fri sten för support. Syftet med migreringen av Microsoft-appar till MSAL är att se till att program varan har en säkerhets förbättring och förbättrade funktioner.

- [Läs vanliga frågor om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Lär dig hur du migrerar appar per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Om du behöver hjälp med att förstå vilka av dina program som använder ADAL rekommenderar vi att du granskar alla dina programs källkod, och om tillämpligt, når oberoende program varu leverantörer eller program leverantörer. Microsoft Support tillhandahåller också en lista över alla ADAL-appar som inte kommer från Microsoft i din klient organisation.

**Migrering av AAD-Graf**

För program som använder AAD Graph följer du våra råd för att [migrera Azure AD-graf-appar till Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Vår check lista för migrering innehåller en komma igång-plats](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Registrerings portalen för Azure-appen visar vilka program som använder AAD Graph. Vi rekommenderar att du granskar alla dina programs källkod och om tillämpligt, nås till alla ISV-eller app-leverantörer. Microsoft Support tillhandahåller också information om all användning av AAD-diagram i din klient organisation.

 










