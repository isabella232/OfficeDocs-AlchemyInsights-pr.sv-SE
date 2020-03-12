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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600402"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Pensionering av äldre eDiscovery-verktyg

Som ett resultat av den nya och förbättrade eDiscovery-funktionen i Microsoft 365 Compliance center kommer följande äldre eDiscovery-verktyg och kommandorattar att dras tillbaka under de kommande månaderna:

- [På plats eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) och [På plats spärrar](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i Exchange administrationscenter.

- Exchange Online PowerShell cmdlets som stöder på plats eDiscovery och På plats håller. (Dessa cmdlets identifieras kollektivt som *-MailboxSearch cmdlets.) Detta inkluderar följande cmdlets:

    - [Ny postlådaSök](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSök](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Ange-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Cmdleten Sök-postlåda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Följande åtgärder i Exchange Web Services API:
    - [FåSökbaraBrevlådor](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOn-brevlådor](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOn-brevlådor](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Avancerad eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje för pensionering:**
- 1 april 2020: Du kan inte skapa nya sökningar och spärrar, men du kan fortfarande köra, redigera och ta bort befintliga sökningar på egen risk. Microsoft Support kommer inte längre att stödja In-Place eDiscovery & Holds i EAC.

- 1 juli 2020: Funktionen & Innehar på plats i EAC placeras i ett skrivskyddat läge. Det innebär att du bara kan ta bort befintliga sökningar och spärrar.

**Mer information finns i**:

 - [Migrera äldre eDiscovery-sökningar och spärrar till Microsoft 365-efterlevnadscentret](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Pensionering av äldre eDiscovery-verktyg](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Vanliga frågor om på plats eDiscovery och På plats håller](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



