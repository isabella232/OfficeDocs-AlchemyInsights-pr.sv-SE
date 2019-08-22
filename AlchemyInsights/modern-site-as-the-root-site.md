---
title: Modern webbplats som rotwebbplatsen
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543871"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="84238-102">Modern webbplats som rotplats</span><span class="sxs-lookup"><span data-stu-id="84238-102">Modern site as root site</span></span>

<span data-ttu-id="84238-103">Vi har börjat introduktionen en ny funktion som gör att du kan byta klassiska webbplats rotplatsen med en modern webbplats.</span><span class="sxs-lookup"><span data-stu-id="84238-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="84238-104">Använd [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta en plats till en annan site under arkivering den ursprungliga webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="84238-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="84238-105">Tillgängligt för både gruppwebbplats (inte ansluten till en grupp) och kommunikation.</span><span class="sxs-lookup"><span data-stu-id="84238-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="84238-106">Ta inte bort klassiska rot-webbplats om du vill skapa en webbplats för modern kommunikation.</span><span class="sxs-lookup"><span data-stu-id="84238-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="84238-107">Detta stöds inte av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="84238-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="84238-108">Ta bort rotwebbplatsen blir alla SharePoint-webbplatser i organisationen inte tillgänglig för alla användare förrän du återställer en webbplats eller skapa en ny webbplats med samma URL.</span><span class="sxs-lookup"><span data-stu-id="84238-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="84238-109">Vi ska kommunicera denna funktion via message center.</span><span class="sxs-lookup"><span data-stu-id="84238-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="84238-110">Du kan förvänta dig funktionen att vara aktiverad i din hyresgäst inom kort.</span><span class="sxs-lookup"><span data-stu-id="84238-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="84238-111">Kända problem med att byta platser</span><span class="sxs-lookup"><span data-stu-id="84238-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="84238-112">Målplatsen kan returnera ett ”hittades inte” fel (HTTP 404) under en kort tid.</span><span class="sxs-lookup"><span data-stu-id="84238-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="84238-113">Innehållet måste vara crawlas igen om du vill uppdatera sökindexet.</span><span class="sxs-lookup"><span data-stu-id="84238-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="84238-114">Det finns inga manuella steg krävs här, detta görs automatiskt.</span><span class="sxs-lookup"><span data-stu-id="84238-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="84238-115">Allt beroende på ”statisk” länkar (till exempel filsynkronisering och OneNote-filer) måste korrigeras manuellt.</span><span class="sxs-lookup"><span data-stu-id="84238-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="84238-116">Project Server-platser kan behöva valideras för att säkerställa att de är fortfarande kopplade på rätt sätt.</span><span class="sxs-lookup"><span data-stu-id="84238-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
