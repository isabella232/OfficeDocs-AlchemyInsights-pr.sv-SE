---
title: Project Online är i skrivskyddat läge
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801670"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="ed326-102">Project Online är i skrivskyddat läge</span><span class="sxs-lookup"><span data-stu-id="ed326-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="ed326-103">Det finns tre vanliga orsaker till varför Project Online kan nå ett skrivskyddat tillstånd:</span><span class="sxs-lookup"><span data-stu-id="ed326-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="ed326-104">Organisationer har bara en licens för Project Online Essentials.</span><span class="sxs-lookup"><span data-stu-id="ed326-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="ed326-105">Det är inte tillräckligt för att du ska kunna behålla webbplatsen, och det tar slutligen slut.</span><span class="sxs-lookup"><span data-stu-id="ed326-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="ed326-106">Vi placerar webbplatsen i skrivskyddat läge så att administratörer vet att något är fel och kan skaffa rätt licenser.</span><span class="sxs-lookup"><span data-stu-id="ed326-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="ed326-107">Administratörer måste lägga till en licens för Project Online Professional och/eller Premium.</span><span class="sxs-lookup"><span data-stu-id="ed326-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="ed326-108">Webbplatsen kommer inte att visas som skrivskyddad.</span><span class="sxs-lookup"><span data-stu-id="ed326-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="ed326-109">Mer information finns i [jämföra lösningar för projekt hantering](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span><span class="sxs-lookup"><span data-stu-id="ed326-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="ed326-110">Den tilldelade kvoten har uppnåtts.</span><span class="sxs-lookup"><span data-stu-id="ed326-110">Assigned quota has been reached.</span></span> <span data-ttu-id="ed326-111">Mer information finns i [Project Web App-kvot](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span><span class="sxs-lookup"><span data-stu-id="ed326-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="ed326-112">Kontrol lera [Konfigurera sammanslagning av tid fas rapporterings data i Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) för att se hur rapporterings granularitet kan påverka kvot användning.</span><span class="sxs-lookup"><span data-stu-id="ed326-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="ed326-113">Skriv skydd kan vara ett tillfälligt tillstånd som kan uppstå under underhållet.</span><span class="sxs-lookup"><span data-stu-id="ed326-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="ed326-114">De flesta underhåll är inte ens uppmärksamma på våra kunder och du kommer inte att se det här, men det finns tillfällen då de korta tids perioder som är skrivskyddade.</span><span class="sxs-lookup"><span data-stu-id="ed326-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
