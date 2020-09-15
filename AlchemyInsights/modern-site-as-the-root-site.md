---
title: Modern webbplats som rotplats
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666888"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="2d8ef-102">Modern webbplats som rotplats</span><span class="sxs-lookup"><span data-stu-id="2d8ef-102">Modern site as root site</span></span>

<span data-ttu-id="2d8ef-103">Vi har börjat använda en ny funktion som gör att du kan [byta till en klassisk webbplats med en modern webbplats](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="2d8ef-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="2d8ef-104">Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats för en webbplats med en annan webbplats när du arkiverar den ursprungliga webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="2d8ef-105">Tillgängligt för både grupp webbplatsen (inte ansluten till en grupp) och kommunikations webbplats.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="2d8ef-106">Ta inte bort den klassiska rot webbplatsen för att skapa en modern kommunikations webbplats.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="2d8ef-107">Det här stöds inte av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="2d8ef-108">Om du tar bort rot webbplatsen kommer alla SharePoint-webbplatser inte att vara tillgängliga för alla användare förrän du återställer webbplatsen eller skapar en ny webbplats på samma URL.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="2d8ef-109">Vi kommer att kommunicera denna funktion via meddelande Center.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="2d8ef-110">Du bör förvänta dig att funktionen är aktive rad i klient organisationen.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="2d8ef-111">Kända problem med att byta plats</span><span class="sxs-lookup"><span data-stu-id="2d8ef-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="2d8ef-112">Mål webbplatsen kan returnera fel meddelandet "inte hittas" (HTTP 404) under en kort tids period.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="2d8ef-113">Innehåll måste crawlas om för att uppdatera Sök indexet.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="2d8ef-114">Det finns inget manuell steg här, detta görs automatiskt.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="2d8ef-115">Allt som är beroende av "statiska" länkar (till exempel filsynkronisering och OneNote-filer) måste åtgärdas manuellt.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="2d8ef-116">Project Server-webbplatser måste kanske val IDE ras för att säkerställa att de är korrekt kopplade.</span><span class="sxs-lookup"><span data-stu-id="2d8ef-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
