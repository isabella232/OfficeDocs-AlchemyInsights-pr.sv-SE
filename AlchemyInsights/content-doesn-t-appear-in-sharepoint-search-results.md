---
title: Innehållet visas inte i SharePoint-sökresultat
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705679"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="8eb55-102">Innehållet visas inte i SharePoint-sökresultat</span><span class="sxs-lookup"><span data-stu-id="8eb55-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="8eb55-103">Följ de här felsökningsstegen när förväntat innehåll inte visas i sökresultaten:</span><span class="sxs-lookup"><span data-stu-id="8eb55-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="8eb55-104">Kontrollera att **webbplatsen** som innehåller det förväntade innehållet är inställd på att tillåta att innehåll visas i sökresultaten.</span><span class="sxs-lookup"><span data-stu-id="8eb55-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="8eb55-105">Följ stegen i [Visa innehåll på en webbplats i sökresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="8eb55-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="8eb55-106">Kontrollera att **listan** eller **biblioteket** som innehåller det förväntade innehållet är inställt på att tillåta att innehåll visas i sökresultaten.</span><span class="sxs-lookup"><span data-stu-id="8eb55-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="8eb55-107">Följ stegen i [Visa innehåll från listor eller bibliotek i sökresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="8eb55-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="8eb55-108">Kontrollera att sidan, dokumentet eller den anpassade sidlayouten har publicerats som en **huvudversion.**</span><span class="sxs-lookup"><span data-stu-id="8eb55-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="8eb55-109">Följ steg 3 i [Sök returnerar inte alla resultat i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="8eb55-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="8eb55-110">Kontrollera att användaren har **behörighet** att visa innehållet.</span><span class="sxs-lookup"><span data-stu-id="8eb55-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="8eb55-111">Följ stegen i [Förstå behörighetsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="8eb55-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="8eb55-112">Om sökschemat har ändrats genom att lägga till en ny hanterad egenskap, genom att redigera en hanterad egenskap eller genom att ta bort en hanterad egenskap krävs det att begära en crawlning och indexera om.</span><span class="sxs-lookup"><span data-stu-id="8eb55-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="8eb55-113">**Indexera** om innehållet genom att följa stegen i [Manuellt begära crawlning och omindexering av en webbplats, ett bibliotek eller en lista](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="8eb55-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="8eb55-114">Detta kan ta ett tag, vänta 24 timmar innan du kontrollerar resultaten igen.</span><span class="sxs-lookup"><span data-stu-id="8eb55-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="8eb55-115">Mer information finns i [Aktivera innehåll på en webbplats som ska vara sökbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="8eb55-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
