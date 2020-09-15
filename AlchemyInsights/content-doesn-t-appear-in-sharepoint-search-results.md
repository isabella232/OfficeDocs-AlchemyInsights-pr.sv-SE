---
title: Innehållet visas inte i Sök resultaten för SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713148"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="788f5-102">Innehållet visas inte i Sök resultaten för SharePoint</span><span class="sxs-lookup"><span data-stu-id="788f5-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="788f5-103">Följ de här fel söknings stegen när förväntat innehåll inte visas i Sök Resultat:</span><span class="sxs-lookup"><span data-stu-id="788f5-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="788f5-104">Kontrol lera att **webbplatsen** som innehåller förväntat innehåll är inställd på att tillåta att innehåll visas i Sök resultaten.</span><span class="sxs-lookup"><span data-stu-id="788f5-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="788f5-105">Följ stegen i [Visa innehåll på en webbplats i Sök resultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="788f5-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="788f5-106">Kontrol lera att **listan** eller **biblioteket** som innehåller förväntat innehåll är inställd på att tillåta att innehåll visas i Sök resultaten.</span><span class="sxs-lookup"><span data-stu-id="788f5-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="788f5-107">Följ stegen i [Visa innehåll från listor eller bibliotek i Sök resultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="788f5-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="788f5-108">Kontrol lera att layouten för sidan, dokumentet eller den anpassade sidan är publicerad som **huvud version.**</span><span class="sxs-lookup"><span data-stu-id="788f5-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="788f5-109">Följ steg 3 i [sökningen returnerar inte alla resultat i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="788f5-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="788f5-110">Kontrol lera att användaren har **behörighet** att visa innehållet.</span><span class="sxs-lookup"><span data-stu-id="788f5-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="788f5-111">Följ stegen i [förstå behörighets nivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="788f5-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="788f5-112">Om sökschemat har ändrats genom att lägga till en ny hanterad egenskap genom att redigera en hanterad egenskap, eller genom att ta bort en hanterad egenskap, krävs en crawlning och ett nytt index.</span><span class="sxs-lookup"><span data-stu-id="788f5-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="788f5-113">**Indexera** om innehållet genom att följa stegen i [manuell crawlning och Omindexering av en webbplats, ett bibliotek eller en lista](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="788f5-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="788f5-114">Det kan ta en stund att vänta 24 timmar innan du kontrollerar resultatet igen.</span><span class="sxs-lookup"><span data-stu-id="788f5-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="788f5-115">För mer information, se [Aktivera innehåll på en webbplats för att vara sökbar](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="788f5-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
