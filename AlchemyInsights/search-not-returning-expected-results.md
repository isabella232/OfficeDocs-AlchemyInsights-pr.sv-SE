---
title: 1491 – sökning-inte returnerar-resultat förväntas
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740492"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="e18d4-102">Innehålls sökning returnerar inte förväntat resultat</span><span class="sxs-lookup"><span data-stu-id="e18d4-102">Content Search not returning expected results</span></span>

<span data-ttu-id="e18d4-103">När du kör innehålls sökningar från Microsoft 365 Security & Compliance Center kan du få oväntade Sök resultat.</span><span class="sxs-lookup"><span data-stu-id="e18d4-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="e18d4-104">Tänk på följande när du kan påverka Sök resultaten:</span><span class="sxs-lookup"><span data-stu-id="e18d4-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="e18d4-105">**Innehålls platser och Sök villkor**: kontrol lera att du har valt rätt innehåll och Sök villkor.</span><span class="sxs-lookup"><span data-stu-id="e18d4-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="e18d4-106">Om du körde en stor sökning (med många platser) bör du dela upp den i flera sökningar.</span><span class="sxs-lookup"><span data-stu-id="e18d4-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="e18d4-107">**Delvis indexerade objekt**:  [delvis indexerade objekt](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) från post lådor ingår i det uppskattade Sök resultatet.</span><span class="sxs-lookup"><span data-stu-id="e18d4-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="e18d4-108">Delvis indexerade objekt från webbplatser i SharePoint och OneDrive tas emellertid inte med i sökningen.</span><span class="sxs-lookup"><span data-stu-id="e18d4-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="e18d4-109">**Sök fel**: när du söker i ett stort antal post lådor (över 100 000-postlådor) kan du få Sök fel, med felkoder som CS008-009 och CS012-002).</span><span class="sxs-lookup"><span data-stu-id="e18d4-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="e18d4-110">I det här fallet ska du försöka med att söka i sökningen igen.</span><span class="sxs-lookup"><span data-stu-id="e18d4-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="e18d4-111">Mer information finns i  [den här artikeln](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="e18d4-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
