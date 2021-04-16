---
title: Äldre eDiscovery-verktyg
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798567"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Äldre eDiscovery-verktyg

Som ett resultat av de nya och förbättrade eDiscovery-funktionerna i efterlevnadscentret för Microsoft 365 kommer följande äldre eDiscovery-verktyg och -kommando att tas bort under de kommande månaderna:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.

- Exchange Online PowerShell-cmdlets som har stöd In-Place eDiscovery och In-Place innehåller. (Dessa cmdlets identifieras gemensamt som cmdlets för *-MailboxSearch.) Det inkluderar följande cmdlets:

    - [Ny postlådesökning](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Cmdlet:en Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.
- Följande åtgärder i API:t för Exchange Web Services:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Tidslinje för retirement**:
- **1 juli 2020** Du kan inte längre skapa nya sökningar och innehåller, men du kan köra, redigera och ta bort befintliga sökningar på egen risk. Microsoft Support stöder inte längre eDiscoveryIn-Place och eDiscovery & i EAC.
    
- **1 oktober 2020** In-Place eDiscovery & Innehåller-funktionen i EAC att placeras i skrivskyddsläge, så du kan bara ta bort befintliga sökningar och inläsningar.

**Mer information finns i:**

 - [Migrera äldre eDiscovery-sökningar och eDiscovery-sökningar till Efterlevnadscenter för Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Utfasning av äldre eDiscovery-verktyg](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Vanliga frågor och svar om eDiscovery In-Place eDiscovery In-Place holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



