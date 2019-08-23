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
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551577"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="3f943-102">Begränsa SharePoint Online till klassiskt läge</span><span class="sxs-lookup"><span data-stu-id="3f943-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="3f943-103">Vissa organisationer kräver fortfarande klassiskt läge erfarenhet.</span><span class="sxs-lookup"><span data-stu-id="3f943-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="3f943-104">Det finns inga planer på att ta bort klassiska läget på en grundläggande nivå, är det inte längre möjligt att begränsa en hel organisation (innehavare) till klassiskt läge för listor och bibliotek.</span><span class="sxs-lookup"><span data-stu-id="3f943-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="3f943-105">Admin har följande alternativ för att hantera enskilda listor och bibliotek i klassiskt läge med detaljerad Slipp växlar som vi tillhandahåller på följande nivåer:</span><span class="sxs-lookup"><span data-stu-id="3f943-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="3f943-106">webbplatssamlingen</span><span class="sxs-lookup"><span data-stu-id="3f943-106">site collection</span></span>
- <span data-ttu-id="3f943-107">webbplats</span><span class="sxs-lookup"><span data-stu-id="3f943-107">site</span></span>
- <span data-ttu-id="3f943-108">listan</span><span class="sxs-lookup"><span data-stu-id="3f943-108">list</span></span>
- <span data-ttu-id="3f943-109">bibliotek</span><span class="sxs-lookup"><span data-stu-id="3f943-109">library</span></span>

<span data-ttu-id="3f943-110">Dessutom kommer listor som använder vissa funktioner och anpassningar som inte stöds av modern fortfarande automatiskt slås till klassiskt läge.</span><span class="sxs-lookup"><span data-stu-id="3f943-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="3f943-111">Börjar 1 April 2019, processen att inaktivera arrendator nivå av moderna lista och bibliotek börjar och fortsätter genom den 31 maj 2019.</span><span class="sxs-lookup"><span data-stu-id="3f943-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="3f943-112">Listor och bibliotek som är i klassiskt läge på grund av hyresgästen Slipp kommer automatiskt flyttas till modern.</span><span class="sxs-lookup"><span data-stu-id="3f943-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="3f943-113">Om du vill ha klassiskt läge finns mer information [här](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) och PnP Powershell instruktion [här](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) som beskriver alternativ och verktyg som du kan använda för att använda den klassiska problem.</span><span class="sxs-lookup"><span data-stu-id="3f943-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
