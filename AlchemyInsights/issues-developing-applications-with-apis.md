---
title: 'Problem med att utveckla program med API: er'
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975019"
---
# <a name="issues-developing-applications-with-apis"></a>Problem med att utveckla program med API: er

Om du vill börja använda Azure Active Directory Graph API läser du [snabb starts guiden för Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) eller Visa den [interaktiva dokumentationen för Azure AD Graph API Reference](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Slut på stöd för Azure Active Directory-autentiseringspaketet (ADAL) och Azure AD Graph API (AAD-diagram)**

**Från den 30 juni 2020,** lägger vi inte till några nya funktioner i ADAL och Azure AD Graph. Vi fortsätter att tillhandahålla tekniska support-och säkerhets uppdateringar men tillhandahåller inte längre funktions uppdateringar.

**Från den 30 juni, 2022**, kommer vi att få support för ADAL och Azure AD-graf och inte längre erbjuda teknisk support eller säkerhets uppdateringar.

Program som använder ADAL i befintliga OS-versioner fortsätter att fungera efter den här tiden men kommer inte att få teknisk support eller säkerhets uppdateringar.

Appar som använder Azure AD Graph efter den här tiden kan inte längre få svar från slut punkten för Azure AD-diagrammet.

**ADAL migrering**

Vi rekommenderar att du uppdaterar till [Microsoft-autentiseringspaketet (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de senaste funktionerna och säkerhets uppdateringarna.

Om du använder Microsoft-appar är det viktigt att Microsoft håller på att migrera sina program till MSAL efter slut för ande av supporten, vilket garanterar att de kommer att få ut så mycket som möjligt av säkerhets-och funktions förbättringar i MSAL.

1. [Läs vanliga frågor om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Lär dig mer om hur du migrerar appar per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Om du behöver hjälp med att förstå vilka av dina program som använder ADAL rekommenderar vi att du granskar alla dina programs källkod och om tillämpligt, nås till alla ISV-eller app-leverantörer. Microsoft Support tillhandahåller också en lista över alla ADAL-appar som inte kommer från Microsoft i din klient organisation.

**Migrering av AAD-Graf**

För program som använder Azure AD Graph följer du våra råd för att migrera [Azure AD-graf-appar till Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Vår check lista för migrering innehåller en komma igång-plats](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Registrerings portalen för Azure-appen visar vilka program som använder AAD Graph. Vi rekommenderar att du granskar alla dina programs källkod och om tillämpligt, nås till alla ISV-eller app-leverantörer. Microsoft-supporten kan också tillhandahålla en lista över alla funktioner i AAD-diagram i klient organisationen.
1. För att ditt program ska kunna komma åt data i Microsoft Graph måste användaren eller administratören ge den rätt behörighet genom godkännande processen. [Behörighets referensen för Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) visar de behörigheter som är kopplade till varje huvud uppsättning med Microsoft Graph API: er. Det ger också vägledning om hur du använder behörigheterna.
