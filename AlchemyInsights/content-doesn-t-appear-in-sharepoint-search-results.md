---
title: Innehåll visas inte i sökresultaten i SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363841"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="af7a5-102">Innehåll visas inte i sökresultaten i SharePoint</span><span class="sxs-lookup"><span data-stu-id="af7a5-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="af7a5-103">Följ dessa felsökningsåtgärder förväntade innehåll inte visas i sökresultat:</span><span class="sxs-lookup"><span data-stu-id="af7a5-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="af7a5-104">Kontrollera att **platsen** som innehåller det förväntade innehållet anges att innehållet ska visas i sökresultaten.</span><span class="sxs-lookup"><span data-stu-id="af7a5-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="af7a5-105">Följ stegen i [Visa innehåll på en webbplats i sökresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="af7a5-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="af7a5-106">Kontrollera att **listan** eller **biblioteket** som innehåller det förväntade innehållet anges att innehållet ska visas i sökresultaten.</span><span class="sxs-lookup"><span data-stu-id="af7a5-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="af7a5-107">Följ stegen i [Visa innehåll från listor eller bibliotek i sökresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="af7a5-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="af7a5-108">Kontrollera sidan, dokumentet eller anpassad sidlayout har publicerats som en **huvudversion.**</span><span class="sxs-lookup"><span data-stu-id="af7a5-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="af7a5-109">Följ steg 3 i [sökningen inte returnera alla resultat i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="af7a5-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="af7a5-110">Kontrollera att användaren har **behörighet** att visa innehållet.</span><span class="sxs-lookup"><span data-stu-id="af7a5-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="af7a5-111">Följ stegen i [Så här fungerar behörighetsnivåer i SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="af7a5-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="af7a5-112">Om Sök-schemat har ändrats genom att lägga till en ny hanterad egenskap, redigera en hanterad egenskap eller ta bort en hanterad egenskap som begär en crawlning och indexera kommer att krävas.</span><span class="sxs-lookup"><span data-stu-id="af7a5-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="af7a5-113">**Indexera** innehåll genom att följa stegen i [begäran manuellt och crawlning omindexering av en webbplats, ett bibliotek eller en lista](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="af7a5-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="af7a5-114">Detta kan ta en stund, vänta 24 timmar innan du kontrollerar resultatet igen.</span><span class="sxs-lookup"><span data-stu-id="af7a5-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="af7a5-115">Mer information finns i [Aktivera innehåll på en webbplats ska vara sökbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="af7a5-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
