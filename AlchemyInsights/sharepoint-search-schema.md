---
title: Hantera sökschemat i SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770569"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="f88c6-102">Hantera sökschemat i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f88c6-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="f88c6-103">Sök schema styr vad användarna kan söka efter, hur användarna kan söka i det och hur du kan presentera resultaten på dina Sök webbplatser.</span><span class="sxs-lookup"><span data-stu-id="f88c6-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="f88c6-104">Se [Hantera sökschemat i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) för att få reda på hur du:</span><span class="sxs-lookup"><span data-stu-id="f88c6-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="f88c6-105">Ändra sökschemat.</span><span class="sxs-lookup"><span data-stu-id="f88c6-105">Change the search schema.</span></span>
- <span data-ttu-id="f88c6-106">Skapa hanterade egenskaper.</span><span class="sxs-lookup"><span data-stu-id="f88c6-106">Create managed properties.</span></span>
- <span data-ttu-id="f88c6-107">Mappa crawlade kart egenskaper till hanterade egenskaper.</span><span class="sxs-lookup"><span data-stu-id="f88c6-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="f88c6-108">Tänk på följande när du hanterar sökschemat:</span><span class="sxs-lookup"><span data-stu-id="f88c6-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="f88c6-109">Om du får en varning om att **programmet har pausats** när du gör en schema ändring är det här bara tillfällig eftersom det finns tjänst underhåll.</span><span class="sxs-lookup"><span data-stu-id="f88c6-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="f88c6-110">Om det finns mer än 24 timmar och du fortfarande upplever varningen kan du logga in ett support ärende.</span><span class="sxs-lookup"><span data-stu-id="f88c6-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="f88c6-111">När du ändrar hanterade egenskaper eller lägger till nya träder ändringarna i kraft först efter att innehållet har crawlats på nytt.</span><span class="sxs-lookup"><span data-stu-id="f88c6-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="f88c6-112">I SharePoint Online sker crawlningen automatiskt baserat på det definierade synkroniseringsschemat.</span><span class="sxs-lookup"><span data-stu-id="f88c6-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="f88c6-113">Om du vill vara säker på att dina ändringar är crawlade kan du [begära en Omindexering av listan eller biblioteket](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="f88c6-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="f88c6-114">En fullständig översikt över sökschemat finns i [Introduktion till sökschemat](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="f88c6-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


