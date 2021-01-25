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
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974766"
---
# <a name="issues-developing-applications"></a>Problem med att utveckla program

För att felsöka de vanligaste problemen när du skapar Azure Active Directory (AD)-program kan du läsa följande artiklar:

- [Jag ser problem med att logga in på program via Chrome-webbläsaren](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Jag vet inte hur man ändrar token för Tokenbegäran för mitt program](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Jag har förvirrat till hur program medgivande fungerar](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Jag vet inte hur jag ger behörighet till mitt program](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Jag förstår inte skillnaden mellan delegerade och program behörigheter](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Slut på stöd för Azure Active Directory-autentiseringspaketet (ADAL) och Azure AD Graph API (AAD-diagram)** _

- Från den 30 juni 2020 lägger vi inte längre till några nya funktioner i Azure Active Directory-autentiseringspaketet (ADAL) och Azure AD Graph API (AAD-diagram). Vi fortsätter att tillhandahålla tekniska support-och säkerhets uppdateringar men tillhandahåller inte längre funktions uppdateringar.

- Från och med den 30 juni 2022 kommer vi att få support för ADAL och AAD-graf och inte längre erbjuda teknisk support eller säkerhets uppdateringar. Som ett resultat av detta villkor gäller följande:

    - Program som använder ADAL i befintliga OS-versioner fortsätter att fungera efter den här tiden men kommer inte att få teknisk support eller säkerhets uppdateringar.

    - Appar som använder AAD Graph efter den här tiden får inte längre svar från slut punkten för en AAD-Graf

_ *ADAL-migrering**

Om du använder Microsoft-appar rekommenderar vi att du uppdaterar till Microsoft-autentiseringspaketet (MSAL), som har de senaste funktionerna och säkerhets uppdateringarna. Denna rekommendation är att Microsoft initierar processen att migrera sina appar till MSAL efter tids fri sten för support. 

Migreringen från Microsoft av sina program till MSAL säkerställer att apparna förbehåller sig från MSALs säkerhets-och funktions förbättringar.

1. [Läs vanliga frågor om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Lär dig hur du migrerar appar per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Om du behöver hjälp med att förstå vilka av dina program som använder ADAL rekommenderar vi att du granskar alla dina programs källkod och, om tillämpligt, kommer ut till någon oberoende program varu leverantör (ISV) eller program leverantör. Microsoft Support tillhandahåller också en lista över alla ADAL-appar som inte kommer från Microsoft i din klient organisation.

**Migrering av AAD-Graf**

För program som använder AAD-diagram följer du vår vägledning för att migrera AAD Graph-appar till Microsoft Graph:

1. [Vår check lista för migrering innehåller en komma igång-plats](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Registrerings portalen för Azure-appen visar vilka program som använder AAD Graph. Vi rekommenderar att du granskar alla dina programs källkod och, om tillämpligt, kommer ut till oberoende program varu leverantörer eller program leverantörer. Microsoft-supporten kan också tillhandahålla information om användning av AAD Graph i din klient organisation.







