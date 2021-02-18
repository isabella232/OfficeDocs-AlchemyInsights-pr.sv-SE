---
title: Hantera externa inställningar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294432"
---
# <a name="managing-external-settings"></a>Hantera externa inställningar

**Meddelande**

- [Utfasning av WebView-inloggningssupport från Google från den 4 januari 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support) Testa om dina appar påverkas av att följa Googles anvisningar om kompatibilitetstestning
- Se till att du använder systemets webbvy eller systemwebbläsare när du loggar in dina användare med Google-konsumentkonton

**Hantera inställningar för inbjudan**

Bekräfta att du [har konfigurerat inställningarna för externt samarbete så](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) att rätt personer kan skicka inbjudningar.

**Hantera behörigheter för gästanvändare**

1. Globala administratörer kan hantera gäståtkomstbehörigheter i katalogen via Azure Portal genom att konfigurera behörigheter för gäståtkomst på sidan Inställningar för externt samarbete. [Läs mer om den här inställningen.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)
2. Om du vill att dina gäster ska få åtkomst till appar som Teams eller SharePoint bekräftar du att du har konfigurerat apparna för att tillåta gäståtkomst. Läs mer om [Teams inställningar och](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [SharePoint.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)

**Konfigurera inbjudningar:**

- [Aktivera B2B externt samarbete och hantera vem som kan bjuda in gäster](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tillåta eller blockera inbjudningar till användare från specifika organisationer](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**Konfigurera tillåtna identitetsproviders:**

- [Google-federation](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Direktfederation](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [E-postautentisering med lösenord](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
