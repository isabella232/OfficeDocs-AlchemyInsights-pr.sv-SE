---
title: Hantera sökschemat i SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042981"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="603e2-102">Hantera sökschemat i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="603e2-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="603e2-103">Sök schemat styr vad användare kan söka efter, hur användare kan söka efter det och hur du kan presentera resultaten på dina sökwebbplatser.</span><span class="sxs-lookup"><span data-stu-id="603e2-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="603e2-104">Se [Hantera sökschemat i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) för att lära dig hur du:</span><span class="sxs-lookup"><span data-stu-id="603e2-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="603e2-105">Ändra sökschemat.</span><span class="sxs-lookup"><span data-stu-id="603e2-105">Change the search schema.</span></span>
- <span data-ttu-id="603e2-106">Skapa hanterade egenskaper.</span><span class="sxs-lookup"><span data-stu-id="603e2-106">Create managed properties.</span></span>
- <span data-ttu-id="603e2-107">Karta crawlad karta crawlade egenskaper till hanterade egenskaper.</span><span class="sxs-lookup"><span data-stu-id="603e2-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="603e2-108">Observera följande när det gäller att hantera ditt sökschema:</span><span class="sxs-lookup"><span data-stu-id="603e2-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="603e2-109">Om du får en varning som anger **att programmet har pausats** när du gör en schemaändring, är detta bara tillfälligt eftersom det finns service underhåll inträffar.</span><span class="sxs-lookup"><span data-stu-id="603e2-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="603e2-110">Om mer än 24 timmar har passerat och du fortfarande upplever varningen, vänligen logga ett supportärende.</span><span class="sxs-lookup"><span data-stu-id="603e2-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="603e2-111">När du ändrar hanterade egenskaper eller lägger till nya, träder ändringarna i kraft först när innehållet har crawlas på nytt.</span><span class="sxs-lookup"><span data-stu-id="603e2-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="603e2-112">I SharePoint Online sker crawlningen automatiskt baserat på det definierade crawlningsschemat.</span><span class="sxs-lookup"><span data-stu-id="603e2-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="603e2-113">Om du vill vara säker på att ändringarna crawlas kan du [begära en Omindexering av listan eller biblioteket](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="603e2-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="603e2-114">En fullständig översikt över sökschemat finns i Introduktion till [sökschemat](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="603e2-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


