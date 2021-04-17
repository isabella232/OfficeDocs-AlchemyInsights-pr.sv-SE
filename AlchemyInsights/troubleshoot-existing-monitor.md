---
title: Felsöka befintlig bildskärm
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824597"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="be24f-102">Felsöka en befintlig bildskärm</span><span class="sxs-lookup"><span data-stu-id="be24f-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="be24f-103">Prova de här lösningarna för att felsöka en bildskärm.</span><span class="sxs-lookup"><span data-stu-id="be24f-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="be24f-104">**Uppdatera bildskärmen:**</span><span class="sxs-lookup"><span data-stu-id="be24f-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="be24f-105">Tryck på följande tangenter samtidigt: Windows-tangenten + Ctrl + Skift + B. Det här uppdaterar kommunikationen med grafikdrivrutinen.</span><span class="sxs-lookup"><span data-stu-id="be24f-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="be24f-106">Bildskärmarna blinkar tillfälligt och kommer tillbaka efter några sekunder.</span><span class="sxs-lookup"><span data-stu-id="be24f-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="be24f-107">**Felsöka maskinvara för bildskärmen:**</span><span class="sxs-lookup"><span data-stu-id="be24f-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="be24f-108">Koppla ur kabeln som ansluter datorn till bildskärmen och anslut den igen.</span><span class="sxs-lookup"><span data-stu-id="be24f-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="be24f-109">Koppla bort alla enheter som inte är nödvändiga från datorn (till exempel adaptrar eller dockor).</span><span class="sxs-lookup"><span data-stu-id="be24f-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="be24f-110">**Om du nyligen har installerat en uppdatering på datorn kan du återställa bildskärmsdrivrutinen:**</span><span class="sxs-lookup"><span data-stu-id="be24f-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="be24f-111">Välj **Start**, **skriv enhetshanteraren** och **välj Enhetshanteraren** i resultatet.</span><span class="sxs-lookup"><span data-stu-id="be24f-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="be24f-112">Expandera avsnittet **Bildskärmskort,** högerklicka på bildskärmskortet och välj **Egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="be24f-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="be24f-113">Gå till fliken **Drivrutin** och välj **Återställ drivrutin.**</span><span class="sxs-lookup"><span data-stu-id="be24f-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="be24f-114">Obs! Om det här inte är tillgängligt eller är nedtonat väljer du **Nej** i alternativen nedan för att gå vidare till nästa steg.</span><span class="sxs-lookup"><span data-stu-id="be24f-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="be24f-115">Du kan behöva starta om datorn innan ändringarna börjar gälla.</span><span class="sxs-lookup"><span data-stu-id="be24f-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="be24f-116">**Avinstallera och installera om din bildskärmsdrivrutin:**</span><span class="sxs-lookup"><span data-stu-id="be24f-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="be24f-117">Välj **Start**, **skriv enhetshanteraren** och **välj Enhetshanteraren** i resultatet.</span><span class="sxs-lookup"><span data-stu-id="be24f-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="be24f-118">Expandera avsnittet **Bildskärmskort,** högerklicka på bildskärmskortet och välj **Avinstallera enhet**.</span><span class="sxs-lookup"><span data-stu-id="be24f-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="be24f-119">Markera rutan bredvid Ta **bort drivrutinsprogramvaran för den här enheten** och välj **Avinstallera**.</span><span class="sxs-lookup"><span data-stu-id="be24f-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="be24f-120">Obs! Du kan bli ombedd att starta om datorn i det här läget.</span><span class="sxs-lookup"><span data-stu-id="be24f-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="be24f-121">Skriv ned resten av instruktionerna innan du startar om.</span><span class="sxs-lookup"><span data-stu-id="be24f-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="be24f-122">Öppna Enhetshanteraren igen.</span><span class="sxs-lookup"><span data-stu-id="be24f-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="be24f-123">Expandera avsnittet **Bildskärmskort,** högerklicka på bildskärmskortet och välj **Uppdatera drivrutin.**</span><span class="sxs-lookup"><span data-stu-id="be24f-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="be24f-124">Välj **Sök automatiskt efter programvara för uppdatering av drivrutinen** och följ installationsanvisningarna.</span><span class="sxs-lookup"><span data-stu-id="be24f-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>