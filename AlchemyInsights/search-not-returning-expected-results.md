---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355895"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="5d513-102">Innehåll sökningen inte ger förväntade resultat</span><span class="sxs-lookup"><span data-stu-id="5d513-102">Content Search not returning expected results</span></span>

<span data-ttu-id="5d513-103">När du kör innehållssökning från Office 365 säkerhet & regelefterlevnadscentret hända oväntade resultat.</span><span class="sxs-lookup"><span data-stu-id="5d513-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="5d513-104">Tänk på följande saker som kan påverka dina sökresultat:</span><span class="sxs-lookup"><span data-stu-id="5d513-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="5d513-105">**Innehållsplatser och sökvillkor**: Kontrollera att du har valt rätt innehållsplatser och sökvillkor.</span><span class="sxs-lookup"><span data-stu-id="5d513-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="5d513-106">Om du körde en stor sökning (med många platser), bör du överväga att dela upp det i flera sökningar.</span><span class="sxs-lookup"><span data-stu-id="5d513-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="5d513-107">**Delvis indexerade objekt**: [delvis indexerade artiklar](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) från postlådor ingår i uppskattade sökresultaten.</span><span class="sxs-lookup"><span data-stu-id="5d513-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="5d513-108">Dock ingår delvis indexerade artiklar från webbplatser i SharePoint och OneDrive inte i uppskattningen sökning.</span><span class="sxs-lookup"><span data-stu-id="5d513-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="5d513-109">**Sök fel**: när du söker ett stort antal postlådor (över 100 000 postlådor), kan du få söka fel med felkoder som CS008-009- och CS012-002).</span><span class="sxs-lookup"><span data-stu-id="5d513-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="5d513-110">Försök i så fall Sök endast efter de misslyckade innehållsplatser.</span><span class="sxs-lookup"><span data-stu-id="5d513-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="5d513-111">Finns i [den här artikeln](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) för mer information.</span><span class="sxs-lookup"><span data-stu-id="5d513-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
