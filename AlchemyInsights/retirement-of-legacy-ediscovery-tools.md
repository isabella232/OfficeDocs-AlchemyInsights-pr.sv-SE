---
title: Dra av äldre eDiscovery-verktyg
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902638"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Dra av äldre eDiscovery-verktyg

Som ett resultat av de nya och förbättrade eDiscovery-funktionerna i Microsoft 365 Compliance Center kommer följande eDiscovery-verktyg och cmdlets att dras tillbaka under de kommande månaderna:

- Lokal [eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) och [plats undantag](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i administrations centret för Exchange.

- PowerShell-cmdlets för Exchange Online som stöder lokal eDiscovery och in-Place-undantag. (De här cmdletarna identifieras tillsammans som *-MailboxSearch cmdlets.) Detta inkluderar följande cmdletar:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stopp-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdleten [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Följande åtgärder i Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Avancerad eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tids linje för tillbakadragning**:
- Den **1 juli 2020** Du kan inte längre skapa nya sökningar och undantag, men du kan köra, redigera och ta bort befintliga sökningar på egen risk. Microsoft Support stöder inte längre eDiscovery på plats & i UK.
    
- Den **1 oktober 2020** In-Place eDiscovery & innehåller funktioner i UK är skrivskyddade, så du kan bara ta bort befintliga sökningar och undantag.

**Mer information finns i**:

 - [Migrera bakåtkompatibla sökningar och undantag till Microsoft 365 Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Utfasning av äldre eDiscovery-verktyg](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Vanliga frågor och svar om eDiscovery-och plats undantag](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



