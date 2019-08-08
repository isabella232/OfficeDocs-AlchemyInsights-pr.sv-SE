---
title: Modern webbplats som rotwebbplatsen
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232733"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="b1b44-102">Modern webbplats som rotplats</span><span class="sxs-lookup"><span data-stu-id="b1b44-102">Modern site as root site</span></span>

<span data-ttu-id="b1b44-103">Vi har börjat introduktionen en ny funktion som gör att du kan byta klassiska webbplats rotplatsen med en modern webbplats.</span><span class="sxs-lookup"><span data-stu-id="b1b44-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="b1b44-104">Använd [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta en plats till en annan site under arkivering den ursprungliga webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="b1b44-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="b1b44-105">Tillgängligt för både gruppwebbplats (inte ansluten till en grupp) och kommunikation.</span><span class="sxs-lookup"><span data-stu-id="b1b44-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="b1b44-106">Ta inte bort klassiska rot-webbplats om du vill skapa en webbplats för modern kommunikation.</span><span class="sxs-lookup"><span data-stu-id="b1b44-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="b1b44-107">Detta stöds inte av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1b44-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="b1b44-108">Ta bort rotwebbplatsen blir alla SharePoint-webbplatser i organisationen inte tillgänglig för alla användare förrän du återställer en webbplats eller skapa en ny webbplats med samma URL.</span><span class="sxs-lookup"><span data-stu-id="b1b44-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="b1b44-109">Vi ska kommunicera denna funktion via message center.</span><span class="sxs-lookup"><span data-stu-id="b1b44-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="b1b44-110">Du kan förvänta dig funktionen att vara aktiverad i din hyresgäst inom kort.</span><span class="sxs-lookup"><span data-stu-id="b1b44-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="b1b44-111">Kända problem med att byta platser</span><span class="sxs-lookup"><span data-stu-id="b1b44-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="b1b44-112">Målplatsen kan returnera ett ”hittades inte” fel (HTTP 404) under en kort tid.</span><span class="sxs-lookup"><span data-stu-id="b1b44-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="b1b44-113">Innehållet måste vara crawlas igen om du vill uppdatera sökindexet.</span><span class="sxs-lookup"><span data-stu-id="b1b44-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="b1b44-114">Det finns inga manuella steg krävs här, detta görs automatiskt.</span><span class="sxs-lookup"><span data-stu-id="b1b44-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="b1b44-115">Allt beroende på ”statisk” länkar (till exempel filsynkronisering och OneNote-filer) måste korrigeras manuellt.</span><span class="sxs-lookup"><span data-stu-id="b1b44-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="b1b44-116">Project Server-platser kan behöva valideras för att säkerställa att de är fortfarande kopplade på rätt sätt.</span><span class="sxs-lookup"><span data-stu-id="b1b44-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
