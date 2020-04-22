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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="01f45-102">Pensionering av Legacy eDiscovery Tools</span><span class="sxs-lookup"><span data-stu-id="01f45-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="01f45-103">Som ett resultat av den nya och förbättrade eDiscovery-funktionen i Microsoft 365 Compliance Center kommer följande äldre eDiscovery-verktyg och kommandosoldater att dras tillbaka under de kommande månaderna:</span><span class="sxs-lookup"><span data-stu-id="01f45-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="01f45-104">[EDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) och [på plats finns i](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) administrationscentret för Exchange.</span><span class="sxs-lookup"><span data-stu-id="01f45-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="01f45-105">Exchange Online PowerShell-cmdlets som stöder eDiscovery och spärrar på plats.</span><span class="sxs-lookup"><span data-stu-id="01f45-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="01f45-106">(Dessa cmdlets identifieras gemensamt som \*-MailboxSearch cmdlets.) Detta inkluderar följande cmdlets:</span><span class="sxs-lookup"><span data-stu-id="01f45-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="01f45-107">Ny-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="01f45-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="01f45-108">Start-mailboxSearch</span><span class="sxs-lookup"><span data-stu-id="01f45-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="01f45-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="01f45-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="01f45-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="01f45-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="01f45-111">Cmdlet för [sökpostlåda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="01f45-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="01f45-112">Följande åtgärder i Exchange Web Services API:</span><span class="sxs-lookup"><span data-stu-id="01f45-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="01f45-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="01f45-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="01f45-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="01f45-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="01f45-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="01f45-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="01f45-116">Avancerad eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="01f45-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="01f45-117">**Tidslinje för pensionering:**</span><span class="sxs-lookup"><span data-stu-id="01f45-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="01f45-118">1 april 2020: Du kan inte skapa nya sökningar och spärrar, men du kan fortfarande köra, redigera och ta bort befintliga sökningar på egen risk.</span><span class="sxs-lookup"><span data-stu-id="01f45-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="01f45-119">Microsoft Support stöder inte längre eDiscovery på plats & innehåller i EAC.</span><span class="sxs-lookup"><span data-stu-id="01f45-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="01f45-120">1 juli 2020: EDiscovery-funktionen på plats & håller i EAC kommer att placeras i skrivskyddat läge.</span><span class="sxs-lookup"><span data-stu-id="01f45-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="01f45-121">Det innebär att du bara kan ta bort befintliga sökningar och spärrar.</span><span class="sxs-lookup"><span data-stu-id="01f45-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="01f45-122">**Mer information finns i:**</span><span class="sxs-lookup"><span data-stu-id="01f45-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="01f45-123">Migrera äldre eDiscovery-sökningar och spärrar till Microsoft 365 compliance center</span><span class="sxs-lookup"><span data-stu-id="01f45-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="01f45-124">Pensionering av äldre verktyg för eDiscovery</span><span class="sxs-lookup"><span data-stu-id="01f45-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="01f45-125">Vanliga frågor om eDiscovery på plats och spärrar på plats</span><span class="sxs-lookup"><span data-stu-id="01f45-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



