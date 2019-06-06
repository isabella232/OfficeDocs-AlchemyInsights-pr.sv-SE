---
title: Hantera search ordlistor i SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736070"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="6a15e-102">Sök i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6a15e-102">Search in SharePoint Online</span></span>

<span data-ttu-id="6a15e-103">Innehållet måste crawlas och lagts till i sökindexet för användare att hitta vad de söker i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="6a15e-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="6a15e-104">Innehållet crawlas automatiskt baserat på en fördefinierad crawlningsschema (crawlningsschema inte kan ändras).</span><span class="sxs-lookup"><span data-stu-id="6a15e-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="6a15e-105">Crawlern hämtar innehåll som har ändrats sedan den senaste crawlningen och uppdaterar indexet.</span><span class="sxs-lookup"><span data-stu-id="6a15e-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="6a15e-106">Följ instruktionerna nedan om du vill kontrollera innehållet crawlas och indexet uppdateras.</span><span class="sxs-lookup"><span data-stu-id="6a15e-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="6a15e-107">Kontrollera att innehållet kan hittas genom att göra innehåll sökbart.</span><span class="sxs-lookup"><span data-stu-id="6a15e-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="6a15e-108">Mer information finns i [Aktivera innehåll på en webbplats ska vara sökbart](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="6a15e-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="6a15e-109">När du har ändrat en hanterad egenskap, eller när du har ändrat avbildningen av crawlade och hanterade vara egenskaper för webbplatsen crawlade igen innan ändringarna återspeglas i sökindexet.</span><span class="sxs-lookup"><span data-stu-id="6a15e-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="6a15e-110">Indexera webbplatsen eftersom ändringarna görs i schemat för sökning och inte till den faktiska platsen, kommer crawlern inte automatiskt.</span><span class="sxs-lookup"><span data-stu-id="6a15e-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="6a15e-111">Mer information finns i [begära manuellt och crawlning omindexering av en webbplats, ett bibliotek eller en lista](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="6a15e-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="6a15e-112">Vänta minst 24 timmar efter att ha begärt manuellt crawla och fullständig indexera och se om du fortfarande har problem.</span><span class="sxs-lookup"><span data-stu-id="6a15e-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="6a15e-113">Om mer än 24 timmar har gått sedan du påbörjade crawla och fullständig indexera, logga ett supportärende.</span><span class="sxs-lookup"><span data-stu-id="6a15e-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="6a15e-114">I många fall kan arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="6a15e-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="6a15e-115">Ge oss minst 24 timmar att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="6a15e-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="6a15e-116">**Viktigt**: om en webbplats, dokument (bibliotek) eller en lista var borttagna och fortfarande visas i sökresultaten, användare får ett fel 404-Filen hittades inte när du försöker komma åt.</span><span class="sxs-lookup"><span data-stu-id="6a15e-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="6a15e-117">Det här problemet ska loggas som ett supportärende för vidare utredning.</span><span class="sxs-lookup"><span data-stu-id="6a15e-117">This issue should be logged as a support case for further investigation.</span></span> 



