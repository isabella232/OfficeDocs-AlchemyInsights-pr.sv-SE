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
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="5e623-102">Pensionering av äldre eDiscovery-verktyg</span><span class="sxs-lookup"><span data-stu-id="5e623-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="5e623-103">Som ett resultat av den nya och förbättrade eDiscovery-funktionen i Microsoft 365 Compliance center kommer följande äldre eDiscovery-verktyg och kommandorattar att dras tillbaka under de kommande månaderna:</span><span class="sxs-lookup"><span data-stu-id="5e623-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="5e623-104">[På plats eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) och [På plats spärrar](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) i Exchange administrationscenter.</span><span class="sxs-lookup"><span data-stu-id="5e623-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="5e623-105">Exchange Online PowerShell cmdlets som stöder på plats eDiscovery och På plats håller.</span><span class="sxs-lookup"><span data-stu-id="5e623-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="5e623-106">(Dessa cmdlets identifieras kollektivt som \*-MailboxSearch cmdlets.) Detta inkluderar följande cmdlets:</span><span class="sxs-lookup"><span data-stu-id="5e623-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="5e623-107">Ny postlådaSök</span><span class="sxs-lookup"><span data-stu-id="5e623-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="5e623-108">Start-MailboxSök</span><span class="sxs-lookup"><span data-stu-id="5e623-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="5e623-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="5e623-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="5e623-110">Ange-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="5e623-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="5e623-111">[Cmdleten Sök-postlåda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) i Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5e623-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="5e623-112">Följande åtgärder i Exchange Web Services API:</span><span class="sxs-lookup"><span data-stu-id="5e623-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="5e623-113">FåSökbaraBrevlådor</span><span class="sxs-lookup"><span data-stu-id="5e623-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="5e623-114">SetHoldOn-brevlådor</span><span class="sxs-lookup"><span data-stu-id="5e623-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="5e623-115">GetHoldOn-brevlådor</span><span class="sxs-lookup"><span data-stu-id="5e623-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="5e623-116">Office 365 Avancerad eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="5e623-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="5e623-117">**Tidslinje för pensionering:**</span><span class="sxs-lookup"><span data-stu-id="5e623-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="5e623-118">1 april 2020: Du kan inte skapa nya sökningar och spärrar, men du kan fortfarande köra, redigera och ta bort befintliga sökningar på egen risk.</span><span class="sxs-lookup"><span data-stu-id="5e623-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="5e623-119">Microsoft Support kommer inte längre att stödja In-Place eDiscovery & Holds i EAC.</span><span class="sxs-lookup"><span data-stu-id="5e623-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="5e623-120">1 juli 2020: Funktionen & Innehar på plats i EAC placeras i ett skrivskyddat läge.</span><span class="sxs-lookup"><span data-stu-id="5e623-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="5e623-121">Det innebär att du bara kan ta bort befintliga sökningar och spärrar.</span><span class="sxs-lookup"><span data-stu-id="5e623-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="5e623-122">**Mer information finns i**:</span><span class="sxs-lookup"><span data-stu-id="5e623-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="5e623-123">Migrera äldre eDiscovery-sökningar och spärrar till Microsoft 365-efterlevnadscentret</span><span class="sxs-lookup"><span data-stu-id="5e623-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="5e623-124">Pensionering av äldre eDiscovery-verktyg</span><span class="sxs-lookup"><span data-stu-id="5e623-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="5e623-125">Vanliga frågor om på plats eDiscovery och På plats håller</span><span class="sxs-lookup"><span data-stu-id="5e623-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



