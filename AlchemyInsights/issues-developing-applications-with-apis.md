---
title: Problem med att utveckla program med API:er
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
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013478"
---
# <a name="issues-developing-applications-with-apis"></a>Problem med att utveckla program med API:er

Om du vill börja använda Azure Active Directory Graph API går du till snabbstartsguiden för [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) eller visar den interaktiva API-referensdokumentationen för Azure AD [Graph.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Support för ADAL (Azure Active Directory) och Azure AD Graph API (AAD Graph)**

**Med start den 30 juni 2020** kommer vi inte längre att lägga till nya funktioner i ADAL och Azure AD Graph. Vi kommer att fortsätta att tillhandahålla teknisk support och säkerhetsuppdateringar men tillhandahåller inte längre funktionsuppdateringar.

**Med start den 30 juni 2022** avslutar vi supporten för ADAL och Azure AD Graph och kommer inte längre att tillhandahålla teknisk support eller säkerhetsuppdateringar.

Appar som använder ADAL i befintliga OS-versioner kommer att fortsätta att fungera efter denna tid, men får ingen teknisk support eller säkerhetsuppdateringar.

Appar som använder Azure AD Graph efter den här tiden kanske inte längre får svar från Azure AD Graph slutpunkten.

**ADAL-migrering**

Vi rekommenderar uppdatering till [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de senaste funktionerna och säkerhetsuppdateringarna.

Om du använder Microsoft-appar vet du att Microsoft håller på att migrera sina program till MSAL innan supporten har löpt ut, så att de kan dra nytta av de kontinuerliga förbättringarna av säkerhet och funktioner i MSAL.

1. [Läs vanliga frågor och svar om ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Läs mer om hur du migrerar appar per plattform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Om du behöver hjälp med att förstå vilken av dina appar som använder ADAL rekommenderar vi att du granskar alla dina appars källkod och, om tillämpligt, kontakta internetleverantörer eller appleverantörer. Microsoft support kan också ge dig en lista med alla ADAL-appar som inte kommer från Microsoft i din klientorganisation.

**AAD Graph-migrering**

För program som använder Azure AD Graph följer du våra riktlinjer för att migrera [Azure AD Graph-appar till Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [I vår checklista för migrering får du en punkt för att komma igång](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Azure-appregistreringsportalen visar vilka program som använder AAD Graph. Vi rekommenderar att du granskar alla dina appars källkod, och om tillämpligt kan du nå ut till ISV:er eller programleverantörer. Microsoft Support kan också ge dig en lista över alla AAD Graph användning i din klient.
1. För att appen ska få åtkomst till data i Microsoft Graph måste användaren eller administratören bevilja den rätt behörigheter via en medgivandeprocess. I [microsoft Graph behörighetsreferensen](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) anges vilka behörigheter som är kopplade till varje huvuduppsättning av Microsofts Graph-API:er. Den innehåller även vägledning om hur du använder behörigheterna.
