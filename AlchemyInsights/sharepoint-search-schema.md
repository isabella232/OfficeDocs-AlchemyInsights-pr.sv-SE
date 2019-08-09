---
title: Hantera schemat för sökning i SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f49195bec64f115063ccfb5256e27fbecd4a54f6
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270155"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="05e13-102">Hantera schemat för sökning i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="05e13-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="05e13-103">Sök schema styr vad användarna kan söka efter, hur användare kan söka och hur du kan presentera resultaten i Sök-webbplatser.</span><span class="sxs-lookup"><span data-stu-id="05e13-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="05e13-104">Se [hantera schemat för sökning i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) och lär dig hur du:</span><span class="sxs-lookup"><span data-stu-id="05e13-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="05e13-105">Ändra schemat för sökning.</span><span class="sxs-lookup"><span data-stu-id="05e13-105">Change the search schema.</span></span>
- <span data-ttu-id="05e13-106">Skapa hanterade egenskaper.</span><span class="sxs-lookup"><span data-stu-id="05e13-106">Create managed properties.</span></span>
- <span data-ttu-id="05e13-107">Datamappning för crawlade mappa crawlade egenskaper till hanterade egenskaper.</span><span class="sxs-lookup"><span data-stu-id="05e13-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="05e13-108">Tänk på följande angående hantera sökning-Schema:</span><span class="sxs-lookup"><span data-stu-id="05e13-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="05e13-109">Om du får en varning om **programmet pausas** när du gör en ändring i schemat, detta är bara tillfälligt som service Underhåll uppstår.</span><span class="sxs-lookup"><span data-stu-id="05e13-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="05e13-110">Logga ett supportärende om mer än 24 timmar har gått och varningen kvarstår.</span><span class="sxs-lookup"><span data-stu-id="05e13-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="05e13-111">När du ändrar hanterade egenskaper eller lägga till nya ändringarna gälla endast när innehållet har crawlade igen.</span><span class="sxs-lookup"><span data-stu-id="05e13-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="05e13-112">I SharePoint Online sker crawlning automatiskt, baserat på definierade crawlningsschema.</span><span class="sxs-lookup"><span data-stu-id="05e13-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="05e13-113">Om du vill vara säker på att ändringarna crawlas, kan du specifikt [begäran omindexering av lista eller bibliotek](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="05e13-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="05e13-114">En fullständig översikt över Sök Schema finns i [Introduktion till Sök Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="05e13-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


