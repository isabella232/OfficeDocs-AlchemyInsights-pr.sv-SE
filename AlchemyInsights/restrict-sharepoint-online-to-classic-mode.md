---
title: Begränsa SharePoint Online till klassiskt läge
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751441"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="f2343-102">Begränsa SharePoint Online till klassiskt läge</span><span class="sxs-lookup"><span data-stu-id="f2343-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="f2343-103">Vissa organisationer kräver fortfarande klassiskt läge.</span><span class="sxs-lookup"><span data-stu-id="f2343-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="f2343-104">Även om det inte finns några planer att ta bort klassiskt läge på en detaljerad nivå är det inte längre möjligt att begränsa en hel organisation (innehavare) till klassiskt läge för listor och bibliotek.</span><span class="sxs-lookup"><span data-stu-id="f2343-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="f2343-105">Administratören har följande alternativ för att hantera enskilda listor och bibliotek i klassiskt läge med hjälp av detaljerade växlar för att avanmäla dem till följande nivåer:</span><span class="sxs-lookup"><span data-stu-id="f2343-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="f2343-106">webbplats samling</span><span class="sxs-lookup"><span data-stu-id="f2343-106">site collection</span></span>
- <span data-ttu-id="f2343-107">webbplatsmallar</span><span class="sxs-lookup"><span data-stu-id="f2343-107">site</span></span>
- <span data-ttu-id="f2343-108">förteckning</span><span class="sxs-lookup"><span data-stu-id="f2343-108">list</span></span>
- <span data-ttu-id="f2343-109">Objektbibliotek</span><span class="sxs-lookup"><span data-stu-id="f2343-109">library</span></span>

<span data-ttu-id="f2343-110">Listor som använder vissa funktioner och anpassningar som inte stöds av moderna kommer att fortsätta att automatiskt växla till klassiskt läge.</span><span class="sxs-lookup"><span data-stu-id="f2343-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="f2343-111">Med början den 1 april 2019, processen för att inaktivera klient organisations nivå avmarkerar du moderna listor och bibliotek startas och fortsätter genom den 31 maj 2019.</span><span class="sxs-lookup"><span data-stu-id="f2343-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="f2343-112">Listor och bibliotek som är i klassiskt läge som ett resultat av att klienter väljer att välja kommer automatiskt att flyttas till moderna.</span><span class="sxs-lookup"><span data-stu-id="f2343-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="f2343-113">Om du behöver klassiskt läge kan du läsa mer [här](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) och PnP PowerShell- [instruktioner som](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) beskriver de alternativ och verktyg som du kan använda i dag för att använda klassiskt läge.</span><span class="sxs-lookup"><span data-stu-id="f2343-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
