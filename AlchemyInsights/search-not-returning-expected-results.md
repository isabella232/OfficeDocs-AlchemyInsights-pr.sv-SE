---
title: 1491-sök-ej-returnera-förväntade-resultat
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510590"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="425a5-102">Innehållssökning returnerar inte förväntade resultat</span><span class="sxs-lookup"><span data-stu-id="425a5-102">Content Search not returning expected results</span></span>

<span data-ttu-id="425a5-103">När du kör Innehållssökningar från Microsoft 365-säkerhetstjänsten & Compliance Center kan du få oväntade sökresultat.</span><span class="sxs-lookup"><span data-stu-id="425a5-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="425a5-104">Tänk på följande saker som kan påverka sökresultaten:</span><span class="sxs-lookup"><span data-stu-id="425a5-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="425a5-105">**Innehållsplatser och sökvillkor**: Kontrollera att du har valt rätt innehållsplatser och sökvillkor.</span><span class="sxs-lookup"><span data-stu-id="425a5-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="425a5-106">Om du har gjort en stor sökning (med många platser) kan du dela upp den i flera sökningar.</span><span class="sxs-lookup"><span data-stu-id="425a5-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="425a5-107">**Delvis indexerade objekt**: [Delvis indexerade objekt](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) från postlådor ingår i de uppskattade sökresultaten.</span><span class="sxs-lookup"><span data-stu-id="425a5-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="425a5-108">Delvis indexerade objekt från webbplatser i SharePoint och OneDrive ingår dock inte i sökninguppskattningen.</span><span class="sxs-lookup"><span data-stu-id="425a5-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="425a5-109">**Sökfel**: När du söker i ett stort antal postlådor (över 100 000 postlådor) kan du få sökfel med felkoder som CS008-009 och CS012-002).</span><span class="sxs-lookup"><span data-stu-id="425a5-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="425a5-110">Försök i det här fallet bara söka efter de misslyckade innehållsplatserna.</span><span class="sxs-lookup"><span data-stu-id="425a5-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="425a5-111">Se [den här artikeln](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) för mer information.</span><span class="sxs-lookup"><span data-stu-id="425a5-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
