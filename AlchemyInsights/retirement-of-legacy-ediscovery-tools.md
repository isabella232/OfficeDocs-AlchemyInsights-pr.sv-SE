---
title: Pensionering av Legacy eDiscovery Tools
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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650586"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensionering av Legacy eDiscovery Tools

Som ett resultat av den nya och förbättrade eDiscovery-funktionen i Microsoft 365 Compliance Center kommer följande äldre eDiscovery-verktyg och kommandosoldater att dras tillbaka under de kommande månaderna:

- [EDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) och [på plats finns i](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) administrationscentret för Exchange.

- Exchange Online PowerShell-cmdlets som stöder eDiscovery och spärrar på plats. (Dessa cmdlets identifieras gemensamt som *-MailboxSearch cmdlets.) Detta inkluderar följande cmdlets:

    - [Ny-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-mailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet för [sökpostlåda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Följande åtgärder i Exchange Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Avancerad eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje för pensionering:**
- 1 april 2020: Du kan inte skapa nya sökningar och spärrar, men du kan fortfarande köra, redigera och ta bort befintliga sökningar på egen risk. Microsoft Support stöder inte längre eDiscovery på plats & innehåller i EAC.

- 1 juli 2020: EDiscovery-funktionen på plats & håller i EAC kommer att placeras i skrivskyddat läge. Det innebär att du bara kan ta bort befintliga sökningar och spärrar.

**Mer information finns i:**

 - [Migrera äldre eDiscovery-sökningar och spärrar till Microsoft 365 compliance center](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensionering av äldre verktyg för eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Vanliga frågor om eDiscovery på plats och spärrar på plats](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



