---
title: Byt ut din klassiska rotwebbplats mot en modern sajt
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
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749278"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="f03a3-102">Byt ut din klassiska rotwebbplats mot en modern sajt</span><span class="sxs-lookup"><span data-stu-id="f03a3-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="f03a3-103">Om din miljö har ställts in före april 2019, kan du ändra din rotwebbplats till en modern webbplats med hjälp av Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f03a3-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="f03a3-104">Om du har en annan webbplats som du vill använda som rotwebbplats kan du ersätta [(byta) rotwebbplatsen](https://docs.microsoft.com/sharepoint/modern-root-site) med den.</span><span class="sxs-lookup"><span data-stu-id="f03a3-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="f03a3-105">Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats på en plats med en annan plats medan du arkiverar den ursprungliga platsen.</span><span class="sxs-lookup"><span data-stu-id="f03a3-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="f03a3-106">Tillgänglig för både gruppwebbplats (inte ansluten till en grupp) och kommunikations plats.</span><span class="sxs-lookup"><span data-stu-id="f03a3-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="f03a3-107">Ytterligare funktioner kommer att introduceras snart som gör att du kan fortsätta att använda innehållet på webbplatsen, men konvertera den befintliga platsen till en kommunikations plats.</span><span class="sxs-lookup"><span data-stu-id="f03a3-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="f03a3-108">Dessa funktioner kommer att rullas ut gradvis.</span><span class="sxs-lookup"><span data-stu-id="f03a3-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="f03a3-109">Fortsätt att kontrollera Office 365 Message Center för uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="f03a3-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="f03a3-110">Kända problem med att byta webbplatser</span><span class="sxs-lookup"><span data-stu-id="f03a3-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="f03a3-111">Målwebbplatsen kan returnera felet "hittades inte" (HTTP 404) under en kort tidsperiod.</span><span class="sxs-lookup"><span data-stu-id="f03a3-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="f03a3-112">Innehållet kommer att behöva återupprepas för att uppdatera sökindexet.</span><span class="sxs-lookup"><span data-stu-id="f03a3-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="f03a3-113">Det finns ingen manuell steg krävs-detta kommer att ske automatiskt.</span><span class="sxs-lookup"><span data-stu-id="f03a3-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="f03a3-114">Allt som är beroende av "statiska" länkar (till exempel filsynkronisering och OneNote-filer) måste korrigeras manuellt.</span><span class="sxs-lookup"><span data-stu-id="f03a3-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="f03a3-115">Om källplatsen var en nyhetswebbplats för organisationen uppdaterar du URL: en.</span><span class="sxs-lookup"><span data-stu-id="f03a3-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="f03a3-116">Få en lista över alla organisationens nyhetssidor.</span><span class="sxs-lookup"><span data-stu-id="f03a3-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="f03a3-117">Project Server-platser kan behöva verifieras för att säkerställa att de fortfarande är korrekt associerade.</span><span class="sxs-lookup"><span data-stu-id="f03a3-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





