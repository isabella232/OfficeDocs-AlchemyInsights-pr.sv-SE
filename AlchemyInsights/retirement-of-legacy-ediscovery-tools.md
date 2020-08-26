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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="c7359-102">Dra av äldre eDiscovery-verktyg</span><span class="sxs-lookup"><span data-stu-id="c7359-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="c7359-103">Som ett resultat av de nya och förbättrade eDiscovery-funktionerna i Microsoft 365 Compliance Center kommer följande eDiscovery-verktyg och cmdlets att dras tillbaka under de kommande månaderna:</span><span class="sxs-lookup"><span data-stu-id="c7359-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="c7359-104">Lokal [eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) och [plats undantag](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i administrations centret för Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7359-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="c7359-105">PowerShell-cmdlets för Exchange Online som stöder lokal eDiscovery och in-Place-undantag.</span><span class="sxs-lookup"><span data-stu-id="c7359-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="c7359-106">(De här cmdletarna identifieras tillsammans som \*-MailboxSearch cmdlets.) Detta inkluderar följande cmdletar:</span><span class="sxs-lookup"><span data-stu-id="c7359-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="c7359-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c7359-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="c7359-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c7359-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="c7359-109">Stopp-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c7359-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="c7359-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c7359-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="c7359-111">Cmdleten [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c7359-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="c7359-112">Följande åtgärder i Exchange Web Services API:</span><span class="sxs-lookup"><span data-stu-id="c7359-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="c7359-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c7359-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="c7359-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c7359-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="c7359-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c7359-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="c7359-116">Avancerad eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="c7359-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="c7359-117">**Tids linje för tillbakadragning**:</span><span class="sxs-lookup"><span data-stu-id="c7359-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="c7359-118">Den **1 juli 2020** Du kan inte längre skapa nya sökningar och undantag, men du kan köra, redigera och ta bort befintliga sökningar på egen risk.</span><span class="sxs-lookup"><span data-stu-id="c7359-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="c7359-119">Microsoft Support stöder inte längre eDiscovery på plats & i UK.</span><span class="sxs-lookup"><span data-stu-id="c7359-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="c7359-120">Den **1 oktober 2020** In-Place eDiscovery & innehåller funktioner i UK är skrivskyddade, så du kan bara ta bort befintliga sökningar och undantag.</span><span class="sxs-lookup"><span data-stu-id="c7359-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="c7359-121">**Mer information finns i**:</span><span class="sxs-lookup"><span data-stu-id="c7359-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="c7359-122">Migrera bakåtkompatibla sökningar och undantag till Microsoft 365 Compliance Center</span><span class="sxs-lookup"><span data-stu-id="c7359-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="c7359-123">Utfasning av äldre eDiscovery-verktyg</span><span class="sxs-lookup"><span data-stu-id="c7359-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="c7359-124">Vanliga frågor och svar om eDiscovery-och plats undantag</span><span class="sxs-lookup"><span data-stu-id="c7359-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



