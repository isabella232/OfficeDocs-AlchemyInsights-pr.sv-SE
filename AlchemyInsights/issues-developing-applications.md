---
title: Problem med att utveckla program
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
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013442"
---
# <a name="issues-developing-applications"></a>Problem med att utveckla program

Information om hur du felsöker de vanligaste problemen Azure Active Directory program (AD) finns i följande artiklar:

- [Jag ser problem med att logga in på program med bara Chrome-webbläsaren](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Jag vet inte hur jag ändrar standard för tokenlivslängd för programmet](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Jag är osäker på hur programmets medgivande fungerar](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Jag vet inte hur jag ska ge behörigheter till programmet](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Jag förstår inte skillnaden mellan delegerade behörigheter och programbehörigheter](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Support för ADAL (Azure Active Directory) och Azure AD Graph API (AAD Graph)***

- Från och med den 30 juni 2020 kommer vi inte längre att lägga till nya funktioner i Azure Active Directory Authentication Library (ADAL) och Azure AD Graph API (AAD Graph). Vi kommer att fortsätta att tillhandahålla teknisk support och säkerhetsuppdateringar men tillhandahåller inte längre funktionsuppdateringar.

- Från och med den 30 juni 2022 avslutar vi supporten för ADAL och AAD Graph och tillhandahåller inte längre teknisk support eller säkerhetsuppdateringar. Resultatet av det här villkoret är konsekvenserna av följande:

    - Appar som använder ADAL i befintliga OS-versioner kommer att fortsätta att fungera efter denna tid, men får ingen teknisk support eller säkerhetsuppdateringar.

    - Appar som använder AAD Graph efter den här tiden kanske inte längre får svar från slutpunkten för AAD Graph

**ADAL-migrering**

Om du använder Microsoft-appar rekommenderar vi att du uppdaterar till Microsoft Authentication Library (MSAL), som har de senaste funktionerna och säkerhetsuppdateringarna. Den här rekommendationen är inom kontexten för att Microsoft initierar processen med att migrera sina appar till MSAL senast tidsgränsen för supporten har löpt ut. 

Genom att Microsoft migrerar sina appar till MSAL ser du till att apparna drar nytta av de ständiga förbättringarna av säkerhet och funktioner i MSAL.

1. [Läs vanliga frågor och svar om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Läs mer om hur du migrerar appar per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Om du behöver hjälp med att förstå vilka appar som använder ADAL rekommenderar vi att du granskar alla dina appars källkod och, om tillämpligt, kontakta någon oberoende programvaruleverantör (ISV) eller appleverantörer. Microsoft support kan också ge dig en lista med alla ADAL-appar som inte kommer från Microsoft i din klientorganisation.

**AAD Graph-migrering**

För program som använder AAD Graph följer du våra riktlinjer för att migrera AAD Graph-appar till Microsoft Graph:

1. [I vår checklista för migrering får du en punkt för att komma igång](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Azure-appregistreringsportalen visar vilka program som använder AAD Graph. Vi rekommenderar att du granskar alla dina apps källkod och, om tillämpligt, kontakta oberoende programvaruleverantörer (ISV) eller appleverantörer. Microsoft Support kan också ge dig information om AAD Graph användning i din klient.







