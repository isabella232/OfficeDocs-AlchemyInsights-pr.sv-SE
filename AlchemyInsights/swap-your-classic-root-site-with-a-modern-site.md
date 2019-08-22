---
title: Byt plats på webbplatsen klassisk rot med en Modern webbplats
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501097"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="d9ed0-102">Byt plats på webbplatsen klassisk rot med en Modern webbplats</span><span class="sxs-lookup"><span data-stu-id="d9ed0-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="d9ed0-103">Om din miljö har registrerat före April 2019 ändra du webbplatsens rot till en modern webbplats med hjälp av Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d9ed0-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="d9ed0-104">Om du har en annan plats som du vill använda som din rotwebbplats kan ersätta du webbplats (swap) roten med den.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="d9ed0-105">Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta en plats till en annan site under arkivering den ursprungliga webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="d9ed0-106">Tillgängligt för både gruppwebbplats (inte ansluten till en grupp) och kommunikation.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="d9ed0-107">Ytterligare funktioner kommer att införas snart som gör att du kan fortsätta använda innehållet på webbplatsen, men konvertera den befintliga webbplatsen till en webbplats för kommunikation.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="d9ed0-108">Dessa funktioner ska slås gradvis.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="d9ed0-109">Fortsätta att kontrollera Office 365 Message Center för uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="d9ed0-110">Kända problem med att byta platser</span><span class="sxs-lookup"><span data-stu-id="d9ed0-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="d9ed0-111">Målplatsen kan returnera ett ”hittades inte” fel (HTTP 404) under en kort tid.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="d9ed0-112">Innehållet måste vara crawlas igen om du vill uppdatera sökindexet.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="d9ed0-113">Det finns inga manuella steg krävs - detta görs automatiskt.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="d9ed0-114">Allt beroende på ”statisk” länkar (till exempel filsynkronisering och OneNote-filer) måste korrigeras manuellt.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="d9ed0-115">Om källwebbplatsen var en organisatorisk nyhetswebbplats, uppdatera URL: en.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="d9ed0-116">Visa en lista över alla webbplatser med nyheter om organisationen.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="d9ed0-117">Project Server-platser kan behöva valideras för att säkerställa att de är fortfarande kopplade på rätt sätt.</span><span class="sxs-lookup"><span data-stu-id="d9ed0-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





