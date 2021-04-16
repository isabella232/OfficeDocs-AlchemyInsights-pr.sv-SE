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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="bad3b-102">Äldre eDiscovery-verktyg</span><span class="sxs-lookup"><span data-stu-id="bad3b-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="bad3b-103">Som ett resultat av de nya och förbättrade eDiscovery-funktionerna i efterlevnadscentret för Microsoft 365 kommer följande äldre eDiscovery-verktyg och -kommando att tas bort under de kommande månaderna:</span><span class="sxs-lookup"><span data-stu-id="bad3b-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="bad3b-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span><span class="sxs-lookup"><span data-stu-id="bad3b-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="bad3b-105">Exchange Online PowerShell-cmdlets som har stöd In-Place eDiscovery och In-Place innehåller.</span><span class="sxs-lookup"><span data-stu-id="bad3b-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="bad3b-106">(Dessa cmdlets identifieras gemensamt som cmdlets för \*-MailboxSearch.) Det inkluderar följande cmdlets:</span><span class="sxs-lookup"><span data-stu-id="bad3b-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="bad3b-107">Ny postlådesökning</span><span class="sxs-lookup"><span data-stu-id="bad3b-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="bad3b-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="bad3b-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="bad3b-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="bad3b-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="bad3b-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="bad3b-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="bad3b-111">[Cmdlet:en Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bad3b-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="bad3b-112">Följande åtgärder i API:t för Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="bad3b-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="bad3b-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="bad3b-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="bad3b-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bad3b-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="bad3b-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bad3b-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="bad3b-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="bad3b-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="bad3b-117">**Tidslinje för retirement**:</span><span class="sxs-lookup"><span data-stu-id="bad3b-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="bad3b-118">**1 juli 2020** Du kan inte längre skapa nya sökningar och innehåller, men du kan köra, redigera och ta bort befintliga sökningar på egen risk.</span><span class="sxs-lookup"><span data-stu-id="bad3b-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="bad3b-119">Microsoft Support stöder inte längre eDiscoveryIn-Place och eDiscovery & i EAC.</span><span class="sxs-lookup"><span data-stu-id="bad3b-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="bad3b-120">**1 oktober 2020** In-Place eDiscovery & Innehåller-funktionen i EAC att placeras i skrivskyddsläge, så du kan bara ta bort befintliga sökningar och inläsningar.</span><span class="sxs-lookup"><span data-stu-id="bad3b-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="bad3b-121">**Mer information finns i:**</span><span class="sxs-lookup"><span data-stu-id="bad3b-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="bad3b-122">Migrera äldre eDiscovery-sökningar och eDiscovery-sökningar till Efterlevnadscenter för Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="bad3b-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="bad3b-123">Utfasning av äldre eDiscovery-verktyg</span><span class="sxs-lookup"><span data-stu-id="bad3b-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="bad3b-124">Vanliga frågor och svar om eDiscovery In-Place eDiscovery In-Place holds</span><span class="sxs-lookup"><span data-stu-id="bad3b-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



