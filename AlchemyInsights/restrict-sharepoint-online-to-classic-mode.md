---
title: Begränsa SharePoint Online till klassiskt läge
ms.author: pebaum
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
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752086"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="78698-102">Begränsa SharePoint Online till klassiskt läge</span><span class="sxs-lookup"><span data-stu-id="78698-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="78698-103">Vissa organisationer kräver fortfarande den klassiska läges upplevelsen.</span><span class="sxs-lookup"><span data-stu-id="78698-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="78698-104">Det finns inga planer på att ta bort klassiskt läge på en detaljerad nivå, men det är inte längre möjligt att begränsa en hel organisation (klient) till klassiskt läge för listor och bibliotek.</span><span class="sxs-lookup"><span data-stu-id="78698-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="78698-105">Administratören kommer att ha följande alternativ för att hantera enskilda listor och bibliotek i klassiskt läge med hjälp av detaljerade opt-out-växlar som vi tillhandahåller på följande nivåer:</span><span class="sxs-lookup"><span data-stu-id="78698-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="78698-106">webbplatssamling</span><span class="sxs-lookup"><span data-stu-id="78698-106">site collection</span></span>
- <span data-ttu-id="78698-107">Webbplats</span><span class="sxs-lookup"><span data-stu-id="78698-107">site</span></span>
- <span data-ttu-id="78698-108">Lista</span><span class="sxs-lookup"><span data-stu-id="78698-108">list</span></span>
- <span data-ttu-id="78698-109">Bibliotek</span><span class="sxs-lookup"><span data-stu-id="78698-109">library</span></span>

<span data-ttu-id="78698-110">Dessutom växlar listor som använder vissa funktioner och anpassningar som inte stöds av modern fortfarande automatiskt till klassiskt läge.</span><span class="sxs-lookup"><span data-stu-id="78698-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="78698-111">Från och med den 1 april 2019, processen för att inaktivera klientnivå välja bort moderna listan och bibliotek startar och fortsätter genom den 31 maj 2019.</span><span class="sxs-lookup"><span data-stu-id="78698-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="78698-112">Listor och bibliotek som är i klassiskt läge som ett resultat av arrendator opt-out kommer automatiskt att flyttas till modern.</span><span class="sxs-lookup"><span data-stu-id="78698-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="78698-113">Om du behöver klassiskt läge se mer information [här](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) och PnP PowerShell-instruktion [här](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) som beskriver alternativ och verktyg som du kan använda i dag för att använda klassisk mode-upplevelse.</span><span class="sxs-lookup"><span data-stu-id="78698-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
