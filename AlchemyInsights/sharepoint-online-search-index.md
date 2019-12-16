---
title: Sök i SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044061"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="f0015-102">Innehåll genomsökning och indexering i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f0015-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="f0015-103">Innehållet måste crawlas och läggas till i sökindexet för att användarna ska kunna hitta det de söker efter i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f0015-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="f0015-104">Innehållet crawlas automatiskt baserat på ett fördefinierat crawlningsschema (crawlningsschemat kan inte ändras).</span><span class="sxs-lookup"><span data-stu-id="f0015-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="f0015-105">Crawlern plockar upp innehåll som har ändrats sedan den senaste crawlningen och uppdaterar indexet.</span><span class="sxs-lookup"><span data-stu-id="f0015-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="f0015-106">Observera följande för att säkerställa att innehållet crawlas och indexet uppdateras:</span><span class="sxs-lookup"><span data-stu-id="f0015-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="f0015-107">Se till att innehållet kan hittas genom [att göra webbplatsens innehåll sökbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="f0015-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="f0015-108">När du har ändrat en hanterad egenskap, eller när du har ändrat mappningen av crawlade och hanterade egenskaper, måste platsen crawlas igen innan ändringarna återspeglas i sökindexet.</span><span class="sxs-lookup"><span data-stu-id="f0015-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="f0015-109">Eftersom dina ändringar görs i sökschemat, och inte på den faktiska platsen, indexerar inte crawlern automatiskt webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="f0015-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="f0015-110">Mer information finns [i begära genomsökning och Omindexering av en webbplats, ett bibliotek eller en lista manuellt](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="f0015-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="f0015-111">Vänta minst 24 timmar efter att du manuellt begärt en crawlning och ett fullständigt nytt index för att se om problemet kvarstår.</span><span class="sxs-lookup"><span data-stu-id="f0015-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="f0015-112">Om mer än 24 timmar har gått sedan du initierade crawlningen och fullständig re-index, vänligen logga ett supportärende.</span><span class="sxs-lookup"><span data-stu-id="f0015-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="f0015-113">I många fall arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="f0015-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f0015-114">Vänligen ge oss minst 24 timmar för att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="f0015-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f0015-115">Om en webbplats, ett dokument (bibliotek) eller en lista har tagits bort och fortfarande visas i sökresultaten, bör användare få ett **fel 404 filen hittades inte** när du försöker komma åt den.</span><span class="sxs-lookup"><span data-stu-id="f0015-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="f0015-116">Det här problemet bör loggas som ett supportärende för ytterligare utredning.</span><span class="sxs-lookup"><span data-stu-id="f0015-116">This issue should be logged as a support case for further investigation.</span></span> 



