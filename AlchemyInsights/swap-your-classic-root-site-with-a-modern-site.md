---
title: Byta till en klassisk rotplats med en modern webbplats
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691197"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="db09e-102">Byta till en klassisk rotplats med en modern webbplats</span><span class="sxs-lookup"><span data-stu-id="db09e-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="db09e-103">Om din miljö installerades före april 2019 kan du ändra din rotplats till en modern webbplats med hjälp av Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="db09e-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="db09e-104">Om du har en annan webbplats som du vill använda som rotplats kan du byta ut [(byta plats) på rot webbplatsen](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="db09e-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="db09e-105">Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats för en webbplats med en annan webbplats när du arkiverar den ursprungliga webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="db09e-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="db09e-106">Tillgängligt för både grupp webbplatsen (inte ansluten till en grupp) och kommunikations webbplats.</span><span class="sxs-lookup"><span data-stu-id="db09e-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="db09e-107">Ytterligare funktioner infogas snart så att du kan fortsätta att använda innehållet på webbplatsen, men konvertera den befintliga webbplatsen till en kommunikations webbplats.</span><span class="sxs-lookup"><span data-stu-id="db09e-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="db09e-108">Dessa funktioner utdelas gradvis.</span><span class="sxs-lookup"><span data-stu-id="db09e-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="db09e-109">Fortsätt att kontrol lera meddelande Center efter uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="db09e-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="db09e-110">Kända problem med att byta plats</span><span class="sxs-lookup"><span data-stu-id="db09e-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="db09e-111">Mål webbplatsen kan returnera fel meddelandet "inte hittas" (HTTP 404) under en kort tids period.</span><span class="sxs-lookup"><span data-stu-id="db09e-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="db09e-112">Innehåll måste crawlas om för att uppdatera Sök indexet.</span><span class="sxs-lookup"><span data-stu-id="db09e-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="db09e-113">Ingen manuell åtgärd krävs – detta görs automatiskt.</span><span class="sxs-lookup"><span data-stu-id="db09e-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="db09e-114">Allt som är beroende av "statiska" länkar (till exempel filsynkronisering och OneNote-filer) måste åtgärdas manuellt.</span><span class="sxs-lookup"><span data-stu-id="db09e-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="db09e-115">Om käll webbplatsen var en webbplats för organisatoriska nyheter uppdaterar du webb adressen.</span><span class="sxs-lookup"><span data-stu-id="db09e-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="db09e-116">Få en lista över alla webbplats nyheter.</span><span class="sxs-lookup"><span data-stu-id="db09e-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="db09e-117">Project Server-webbplatser måste kanske val IDE ras för att säkerställa att de är korrekt kopplade.</span><span class="sxs-lookup"><span data-stu-id="db09e-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
