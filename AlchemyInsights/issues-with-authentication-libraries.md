---
title: Problem med autentiseringsbibliotek
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063700"
---
# <a name="issues-with-authentication-libraries"></a>Problem med autentiseringsbibliotek

1. [Autentiseringsbibliotek för Microsoft-identitetsplattformen](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) listar Microsoft-stödda och kompatibla bibliotek för klient- och mellanprogramsautentisering.
2. Microsoft Authentication Library (MSAL) har stöd för flera [autentiseringsflöden](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) för användning i olika programscenarier.
3. Om du vill autentisera och skaffa token initierar du ett nytt offentligt eller konfidentiellt klientprogram i koden. Du kan ange flera konfigurationsalternativ när du initierar klientappen i Microsoft Authentication Library (MSAL). Mer information finns i [Programkonfigurationsalternativ.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Support för Azure Active Directory Authentication Library (ADAL) och Azure AD Graph API (AAD Graph)**

**Från och med den 30 juni 2020** kommer vi inte längre att lägga till nya funktioner i ADAL och Azure AD Graph. Vi kommer att fortsätta att tillhandahålla teknisk support och säkerhetsuppdateringar men tillhandahåller inte längre funktionsuppdateringar.

**Med början den 30 juni 2022** kommer vi att avsluta supporten för ADAL och Azure AD Graph och kommer inte längre att tillhandahålla teknisk support eller säkerhetsuppdateringar.

Appar som använder ADAL på befintliga OS-versioner fortsätter att fungera efter den här tiden men får *ingen teknisk support eller säkerhetsuppdateringar.*

Appar som använder Azure AD Graph efter den här tiden kanske inte längre får svar från Azure AD Graph-slutpunkten.

**ADAL-migrering**

Vi rekommenderar uppdatering till [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de senaste funktionerna och säkerhetsuppdateringarna.

Om du använder Microsoft-appar vet du att Microsoft arbetar med att migrera programmen till MSAL innan tidsgränsen för supporten löper ut, vilket säkerställer att de kommer att dra nytta av MSAL:s kontinuerliga förbättringar av säkerhet och funktioner.

Mer information finns i:

1. [Läs vanliga frågor och svar om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Läs mer om hur du migrerar appar per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Om du behöver hjälp med att förstå vilka av dina appar som använder ADAL rekommenderar vi att du går igenom alla dina apps källkod och, om tillämpligt, kontakta internetleverantörer eller internetleverantörer. Microsoft support kan också ge dig en lista med alla ADAL-appar som inte kommer från Microsoft i din klientorganisation.

**AAD Graph-migrering**

För program som använder Azure AD Graph följer du våra riktlinjer för att [migrera Azure AD Graph-appar till Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Vår migreringschecklista ger dig en utgångspunkt.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure-appregistreringsportalen visar vilka program som använder AAD Graph. Vi rekommenderar att du granskar alla dina appars källkod, och om tillämpligt kan du nå ut till ISV:er eller programleverantörer. Microsofts support kan också ge dig en lista över all AAD Graph-användning i din klientorganisation.
3. För att appen ska kunna komma åt data i Microsoft Graph måste användaren eller administratören bevilja den rätt behörighet via en medgivandeprocess. I [behörighetsreferensen för Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) visas behörigheterna som är kopplade till varje huvuduppsättning Microsoft Graph-API:er. Den innehåller även vägledning om hur du använder behörigheterna.
