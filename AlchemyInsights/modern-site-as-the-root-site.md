---
title: Modern sajt som root site
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
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753922"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="64112-102">Modern sajt som root site</span><span class="sxs-lookup"><span data-stu-id="64112-102">Modern site as root site</span></span>

<span data-ttu-id="64112-103">Vi har börjat utbyggnaden en ny funktion som gör att du kan [byta din klassiska webbplats rotwebbplats med en modern webbplats](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="64112-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="64112-104">Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats på en plats med en annan plats medan du arkiverar den ursprungliga platsen.</span><span class="sxs-lookup"><span data-stu-id="64112-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="64112-105">Tillgänglig för både gruppwebbplats (inte ansluten till en grupp) och kommunikations plats.</span><span class="sxs-lookup"><span data-stu-id="64112-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="64112-106">Ta inte bort din klassiska rotwebbplats för att skapa en modern kommunikations plats.</span><span class="sxs-lookup"><span data-stu-id="64112-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="64112-107">Detta stöds inte av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="64112-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="64112-108">Om du tar bort rotwebbplatsen blir alla SharePoint-webbplatser i organisationen otillgängliga för alla användare, tills du återställer webbplatsen eller skapar en ny plats på samma webbadress.</span><span class="sxs-lookup"><span data-stu-id="64112-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="64112-109">Vi kommunicerar den här funktionen via Message Center.</span><span class="sxs-lookup"><span data-stu-id="64112-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="64112-110">Du bör förvänta dig att funktionen ska aktiveras i din klient inom kort.</span><span class="sxs-lookup"><span data-stu-id="64112-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="64112-111">Kända problem med att byta webbplatser</span><span class="sxs-lookup"><span data-stu-id="64112-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="64112-112">Målwebbplatsen kan returnera felet "hittades inte" (HTTP 404) under en kort tidsperiod.</span><span class="sxs-lookup"><span data-stu-id="64112-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="64112-113">Innehållet kommer att behöva återupprepas för att uppdatera sökindexet.</span><span class="sxs-lookup"><span data-stu-id="64112-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="64112-114">Det finns inget manuellt steg som krävs här, detta kommer att ske automatiskt.</span><span class="sxs-lookup"><span data-stu-id="64112-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="64112-115">Allt som är beroende av "statiska" länkar (till exempel filsynkronisering och OneNote-filer) måste korrigeras manuellt.</span><span class="sxs-lookup"><span data-stu-id="64112-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="64112-116">Project Server-platser kan behöva verifieras för att säkerställa att de fortfarande är korrekt associerade.</span><span class="sxs-lookup"><span data-stu-id="64112-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
