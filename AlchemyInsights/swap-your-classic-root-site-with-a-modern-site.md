---
title: Byt din klassiska rotplats med en modern webbplats
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741562"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="ddd47-102">Byt din klassiska rotplats med en modern webbplats</span><span class="sxs-lookup"><span data-stu-id="ddd47-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="ddd47-103">Om din miljö har konfigurerats före april 2019 kan du ändra rotplatsen till en modern webbplats med hjälp av Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ddd47-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="ddd47-104">Om du har en annan plats som du vill använda som rotplats kan du ersätta [(byta) rotplatsen](https://docs.microsoft.com/sharepoint/modern-root-site) med den.</span><span class="sxs-lookup"><span data-stu-id="ddd47-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="ddd47-105">Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats på en plats med en annan plats medan du arkiverar den ursprungliga platsen.</span><span class="sxs-lookup"><span data-stu-id="ddd47-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="ddd47-106">Tillgänglig för både gruppwebbplats (inte ansluten till en grupp) och kommunikationswebbplats.</span><span class="sxs-lookup"><span data-stu-id="ddd47-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="ddd47-107">Ytterligare funktioner kommer att införas snart som gör att du kan fortsätta använda innehållet på webbplatsen, men konvertera den befintliga platsen till en kommunikationswebbplats.</span><span class="sxs-lookup"><span data-stu-id="ddd47-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="ddd47-108">Dessa funktioner kommer att rullas ut gradvis.</span><span class="sxs-lookup"><span data-stu-id="ddd47-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="ddd47-109">Fortsätt att söka efter uppdateringar i Meddelandecenter.</span><span class="sxs-lookup"><span data-stu-id="ddd47-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="ddd47-110">Kända problem med att byta webbplatser</span><span class="sxs-lookup"><span data-stu-id="ddd47-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="ddd47-111">Målplatsen kan returnera ett HTTP 404-fel (inte hittats" (HTTP 404) under en kort tidsperiod.</span><span class="sxs-lookup"><span data-stu-id="ddd47-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="ddd47-112">Innehållet måste testas igen för att uppdatera sökindexet.</span><span class="sxs-lookup"><span data-stu-id="ddd47-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="ddd47-113">Det finns inget manuellt steg som krävs - detta kommer att göras automatiskt.</span><span class="sxs-lookup"><span data-stu-id="ddd47-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="ddd47-114">Allt som är beroende av "statiska" länkar (till exempel Filsynkronisering och OneNote-filer) måste korrigeras manuellt.</span><span class="sxs-lookup"><span data-stu-id="ddd47-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="ddd47-115">Om källwebbplatsen var en organisationsnyhetswebbplats uppdaterar du webbadressen.</span><span class="sxs-lookup"><span data-stu-id="ddd47-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="ddd47-116">Få en lista över alla organisationsnyhetswebbplatser.</span><span class="sxs-lookup"><span data-stu-id="ddd47-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="ddd47-117">Project Server-platser kan behöva valideras för att säkerställa att de fortfarande är korrekt associerade.</span><span class="sxs-lookup"><span data-stu-id="ddd47-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
