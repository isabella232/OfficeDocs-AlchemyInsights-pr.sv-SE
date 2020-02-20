---
title: Pensionering av äldre eDiscovery-verktyg
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
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157732"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensionering av äldre eDiscovery-verktyg

Som ett resultat av den nya och förbättrade eDiscovery-funktionen i Microsoft 365 Compliance Center kommer följande äldre eDiscovery-verktyg och kommandosoldater att dras tillbaka under de kommande månaderna:

- [EDiscovery-](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) och [på plats håller](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i administrationscentret för Exchange.

- Exchange Online PowerShell-cmdlets som stöder eDiscovery- och in-Place-spärrar. (Dessa cmdlets identifieras kollektivt som *-MailboxSearch cmdlets.) Detta inkluderar följande cmdlets:

    - [Ny postlådesökning](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Sök efter startpostiepost](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Sökning i uppsättningpostlåda](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Search-Mailbox-cmdlet](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Följande åtgärder i Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Avancerad eDiscovery v1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje för pensionering:**
- 1 april 2020: Du kommer inte att kunna skapa nya sökningar och spärrar, men du kan fortfarande köra, redigera och ta bort befintliga sökningar på egen risk. Microsoft Support stöder inte längre eDiscovery & håller i EAC.

- 1 juli 2020: EDiscovery & innehar funktionalitet i EAC placeras i ett skrivskyddat läge. Det innebär att du bara kan ta bort befintliga sökningar och spärrar.

**Mer information finns i:**

 - [Migrera äldre eDiscovery-sökningar och spärrar till Microsoft 365-efterlevnadscenter](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensionering av äldre eDiscovery-verktyg](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Vanliga frågor om eDiscovery- och in-place-spärrar på plats](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



