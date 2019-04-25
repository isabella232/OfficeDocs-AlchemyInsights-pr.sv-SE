---
title: Begränsa SharePoint Online till klassiskt läge
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32422193"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="7692b-102">Begränsa SharePoint Online till klassiskt läge</span><span class="sxs-lookup"><span data-stu-id="7692b-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="7692b-103">Vissa organisationer kräver fortfarande klassiskt läge erfarenhet.</span><span class="sxs-lookup"><span data-stu-id="7692b-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="7692b-104">Det finns inga planer på att ta bort klassiska läget på en grundläggande nivå, startar April 1,2019, det kommer inte längre vara möjligt att begränsa en hel organisation (innehavare) till klassiskt läge för listor och bibliotek.</span><span class="sxs-lookup"><span data-stu-id="7692b-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="7692b-105">Admin har följande alternativ för att hantera enskilda listor och bibliotek i klassiskt läge med detaljerad Slipp växlar som vi tillhandahåller på följande nivåer:</span><span class="sxs-lookup"><span data-stu-id="7692b-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="7692b-106">webbplatssamlingen</span><span class="sxs-lookup"><span data-stu-id="7692b-106">site collection</span></span>
- <span data-ttu-id="7692b-107">webbplats</span><span class="sxs-lookup"><span data-stu-id="7692b-107">site</span></span>
- <span data-ttu-id="7692b-108">listan</span><span class="sxs-lookup"><span data-stu-id="7692b-108">list</span></span>
- <span data-ttu-id="7692b-109">bibliotek</span><span class="sxs-lookup"><span data-stu-id="7692b-109">library</span></span>

<span data-ttu-id="7692b-110">Dessutom kommer listor som använder vissa funktioner och anpassningar som inte stöds av modern fortfarande automatiskt slås till klassiskt läge.</span><span class="sxs-lookup"><span data-stu-id="7692b-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="7692b-111">Efter den 1 April hanteras listor och bibliotek som är i klassiskt läge på grund av hyresgästen välja bort automatiskt på webbplatsnivå och nivå.</span><span class="sxs-lookup"><span data-stu-id="7692b-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="7692b-112">Om du vill ha klassiskt läge finns mer information här och PnP Powershell instruktion här som beskriver verktyg och alternativ du kan använda för att förbereda för borttagning av en arrendator nivå Slipp den 1 April.</span><span class="sxs-lookup"><span data-stu-id="7692b-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
