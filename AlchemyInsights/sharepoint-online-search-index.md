---
title: Sök i SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507649"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="cf526-102">Spindlar och indexering i SharePoint Online-innehåll</span><span class="sxs-lookup"><span data-stu-id="cf526-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="cf526-103">Innehållet måste crawlas och lagts till i sökindexet för användare att hitta vad de söker i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="cf526-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="cf526-104">Innehållet crawlas automatiskt baserat på en fördefinierad crawlningsschema (crawlningsschema inte kan ändras).</span><span class="sxs-lookup"><span data-stu-id="cf526-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="cf526-105">Crawlern hämtar innehåll som har ändrats sedan den senaste crawlningen och uppdaterar indexet.</span><span class="sxs-lookup"><span data-stu-id="cf526-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="cf526-106">Tänk på följande om du vill kontrollera innehållet crawlas och indexet uppdateras:</span><span class="sxs-lookup"><span data-stu-id="cf526-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="cf526-107">Kontrollera att innehållet kan hittas genom [att skapa sökbara innehåll](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="cf526-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="cf526-108">När du har ändrat en hanterad egenskap, eller när du har ändrat avbildningen av crawlade och hanterade vara egenskaper för webbplatsen crawlade igen innan ändringarna återspeglas i sökindexet.</span><span class="sxs-lookup"><span data-stu-id="cf526-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="cf526-109">Indexera webbplatsen eftersom ändringarna görs i schemat för sökning och inte till den faktiska platsen, kommer crawlern inte automatiskt.</span><span class="sxs-lookup"><span data-stu-id="cf526-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="cf526-110">Mer information finns i [begära manuellt och crawlning omindexering av en webbplats, ett bibliotek eller en lista](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="cf526-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="cf526-111">Vänta minst 24 timmar efter att ha begärt manuellt crawla och fullständig indexera och se om du fortfarande har problem.</span><span class="sxs-lookup"><span data-stu-id="cf526-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="cf526-112">Om mer än 24 timmar har gått sedan du påbörjade crawla och fullständig indexera, logga ett supportärende.</span><span class="sxs-lookup"><span data-stu-id="cf526-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="cf526-113">I många fall kan arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="cf526-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="cf526-114">Ge oss minst 24 timmar att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="cf526-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cf526-115">Om en webbplats har tagits bort (bibliotek)-dokument eller en lista och fortfarande visas i sökresultat, användare får ett **Fel 404 filen inte hittas** när du försöker komma åt den.</span><span class="sxs-lookup"><span data-stu-id="cf526-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="cf526-116">Det här problemet ska loggas som ett supportärende för vidare utredning.</span><span class="sxs-lookup"><span data-stu-id="cf526-116">This issue should be logged as a support case for further investigation.</span></span> 



