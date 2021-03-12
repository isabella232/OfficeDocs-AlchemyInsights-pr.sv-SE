---
title: Problem med Microsoft Graph API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714515"
---
# <a name="microsoft-graph-api-issues"></a>Problem med Microsoft Graph API

Det här avsnittet kan även gälla för utvecklare som fortfarande använder Azure AD Graph API. Vi rekommenderar dock **starkt att** du använder Microsoft Graph för alla scenarier för katalog-, identitets- och åtkomsthantering.

**Autentiserings- eller auktoriseringsproblem**

- Om din app inte kan hämta **token för** att anropa Microsoft Graph väljer du Problem med att hämta en åtkomsttoken **(autentisering)** Microsoft Graph-kategori för att få mer specifik hjälp och support i det här avsnittet.
- Om appen får **401- eller 403-auktoriseringsfel** när du ringer Microsoft Graph väljer du kategorin Få ett felmeddelande om nekad åtkomst **(auktorisering)** Microsoft Graph API för att få mer specifik hjälp och support för det här avsnittet.

**Jag vill använda Microsoft Graph, men vet inte var jag ska börja**

- [Översikt över Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Översikt över hantering av identitet och åtkomst i Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Komma igång med att skapa Microsoft Graph-appar](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – Testa Microsoft Graph-API:er i klientorganisationen eller en demoklientorganisation

**Jag vill använda Microsoft Graph, men har det stöd för de v1.0-katalog-API:er jag behöver?**

Microsoft Graph är det rekommenderade API:t för hantering av katalog, identitet och åtkomst. Det finns dock fortfarande några luckor mellan vad som är möjligt i Azure AD Graph och Microsoft Graph. Läs följande artiklar, som tar upp de senaste skillnaderna som kan vara till hjälp för ditt val:

- [Skillnader i resurstyper mellan Azure AD Graph och Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Skillnader i egenskap mellan Azure AD Graph och Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Skillnader i metod mellan Azure AD och Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API:t som jag anropar fungerar inte – var kan jag testa mer?**

**Microsoft Graph Explorer** – Testa Microsoft Graph API:er i din klientorganisation eller en demoklientorganisation och ta även en titta på exempelfrågorna **i** Microsoft Graph Explorer.

**Min app är för långsam och begränsas också. Vilka förbättringar kan jag göra?**

Beroende på ditt scenario finns det ett antal olika alternativ som du har tillgång till för att göra programmet mer mer uttjänat, och i vissa fall mindre beivrat att begränsas av tjänsten (när du ringer för många samtal).

- [Metodtips för Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Grupperingsförfrågningar](https://docs.microsoft.com/graph/json-batching)
- [Spåra ändringar via deltafråga](https://docs.microsoft.com/graph/delta-query-overview)
- [Få ett meddelande om ändringar via webhooks](https://docs.microsoft.com/graph/webhooks)
- [Begränsningsvägledning](https://docs.microsoft.com/graph/throttling)

**Var hittar jag mer information om fel och kända problem?**

- [Information om Microsoft Graph-felsvar](https://docs.microsoft.com/graph/errors)
- [Kända problem med Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Var kan jag kontrollera status för tjänstens tillgänglighet och anslutning?**

Tjänstens tillgänglighet och anslutning för underliggande tjänster som kan nås via Microsoft Graph kan påverka den övergripande tillgängligheten och prestandan för Microsoft Graph.

- För Azure Active Directory-tjänstens hälsa kontrollerar du statusen för **Säkerhets- och identitetstjänster** som visas på [Azure-statussidan.](https://azure.microsoft.com/status/)
- För Office-tjänster som bidrar till Microsoft Graph kontrollerar du statusen för tjänster som visas på [Hälsoinstrumentpanelen för Office.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph-auktoriseringsfel kan vara ett resultat av flera olika problem, varav de flesta genererar ett 401- eller 403-fel. Följande kan till exempel leda till auktoriseringsfel:

- Felaktiga [förvärvsflöden av åtkomsttoken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Dåligt konfigurerade [behörighetsomfattningar](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Brist på [medgivande](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Supporten upphör för ADAL (Azure Active Directory Authentication Library) och Azure AD Graph API (AAD Graph)_* _

_*Från och med den 30 juni 2020**, kommer vi inte längre att lägga till nya funktioner i ADAL och Azure AD Graph. Vi kommer att fortsätta att tillhandahålla teknisk support och säkerhetsuppdateringar men tillhandahåller inte längre funktionsuppdateringar.

**Med början den 30 juni 2022** kommer vi att avsluta supporten för ADAL och Azure AD Graph och kommer inte längre att tillhandahålla teknisk support eller säkerhetsuppdateringar.

Appar som använder ADAL på befintliga OS-versioner fortsätter att fungera efter den här tiden men får *ingen teknisk support eller säkerhetsuppdateringar.*

Appar som använder Azure AD Graph efter den här tiden kanske inte längre får svar från Azure AD Graph-slutpunkten.

**ADAL-migrering**

Vi rekommenderar uppdatering till [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de senaste funktionerna och säkerhetsuppdateringarna.

Om du använder Microsoft-appar vet du att Microsoft migrerar sina program till MSAL innan tidsgränsen för supporten löper ut, vilket säkerställer att de kommer att dra nytta av MSAL:s kontinuerliga förbättringar av säkerhet och funktioner.

1. [Läs vanliga frågor och svar om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Läs mer om hur du migrerar appar per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Om du behöver hjälp med att förstå vilka av dina appar som använder ADAL rekommenderar vi att du går igenom alla dina apps källkod och, om tillämpligt, kontakta internetleverantörer eller internetleverantörer. Microsoft support kan också ge dig en lista med alla ADAL-appar som inte kommer från Microsoft i din klientorganisation.

**AAD Graph-migrering**

För program som använder Azure AD Graph följer du våra riktlinjer för att [migrera Azure AD Graph-appar till Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [I vår checklista för migrering får du en punkt för att komma igång](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Azure-appregistreringsportalen visar vilka program som använder AAD Graph. Vi rekommenderar att du granskar alla dina appars källkod, och om tillämpligt kan du nå ut till ISV:er eller programleverantörer. Microsoft Support kan också ge dig en lista över all AAD Graph-användning i din klientorganisation.
3. För att appen ska kunna komma åt data i Microsoft Graph måste användaren eller administratören bevilja den rätt behörighet via en medgivandeprocess. I [behörighetsreferensen för Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) visas behörigheterna som är kopplade till varje huvuduppsättning Microsoft Graph-API:er. Den innehåller även vägledning om hur du använder behörigheterna.
