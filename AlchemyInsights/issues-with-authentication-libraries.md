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
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028022"
---
# <a name="issues-with-authentication-libraries"></a>Problem med autentiseringsbibliotek

1. [Microsofts identitetsplattform för autentiseringsbibliotek](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) visar microsoft-stödda och kompatibla klient- och mellanprogramsbibliotek.
2. Microsoft Authentication Library (MSAL) har stöd för flera [autentiseringsflöden](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) för olika programscenarier.
3. Om du vill autentisera och hämta token initierar du ett nytt offentligt eller konfidentiellt klientprogram i koden. Du kan ange flera konfigurationsalternativ när du initierar klientappen i Microsoft Authentication Library (MSAL). Mer information finns i [Programkonfigurationsalternativ](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Support för ADAL (Azure Active Directory) och Azure AD Graph API (AAD Graph)**

**Med start den 30 juni 2020** kommer vi inte längre att lägga till nya funktioner i ADAL och Azure AD Graph. Vi kommer att fortsätta att tillhandahålla teknisk support och säkerhetsuppdateringar men tillhandahåller inte längre funktionsuppdateringar.

**Med start den 30 juni 2022** avslutar vi supporten för ADAL och Azure AD Graph och kommer inte längre att tillhandahålla teknisk support eller säkerhetsuppdateringar.

Appar som använder ADAL på befintliga OS-versioner fortsätter att fungera efter denna tid men får *ingen teknisk support eller säkerhetsuppdateringar.*

Appar som använder Azure AD Graph efter den här tiden kanske inte längre får svar från Azure AD Graph slutpunkten.

**ADAL-migrering**

Vi rekommenderar uppdatering till [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de senaste funktionerna och säkerhetsuppdateringarna.

Om du använder Microsoft-appar vet du att Microsoft håller på att migrera sina program till MSAL innan supporten har löpt ut, vilket säkerställer att de kommer att dra nytta av de kontinuerliga förbättringarna av säkerhet och funktioner i MSAL.

Mer information finns i:

1. [Läs vanliga frågor och svar om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Läs mer om hur du migrerar appar per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Om du behöver hjälp med att förstå vilken av dina appar som använder ADAL rekommenderar vi att du granskar alla dina appars källkod och, om tillämpligt, kontakta internetleverantörer eller appleverantörer. Microsoft support kan också ge dig en lista med alla ADAL-appar som inte kommer från Microsoft i din klientorganisation.

**AAD Graph-migrering**

För program som använder Azure AD Graph följer du våra riktlinjer för att [migrera Azure AD Graph-appar till Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Migreringschecklistan ger dig en utgångspunkt.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure-appregistreringsportalen visar vilka program som använder AAD Graph. Vi rekommenderar att du granskar alla dina appars källkod, och om tillämpligt kan du nå ut till ISV:er eller programleverantörer. Microsoft Support kan också ge dig en lista över alla AAD Graph användning i din klient.
3. För att appen ska få åtkomst till data i Microsoft Graph måste användaren eller administratören bevilja den rätt behörigheter via en medgivandeprocess. I [microsoft Graph behörighetsreferensen](https://docs.microsoft.com/graph/permissions-reference) anges vilka behörigheter som är kopplade till varje huvuduppsättning av Microsofts Graph-API:er. Den innehåller även vägledning om hur du använder behörigheterna.
