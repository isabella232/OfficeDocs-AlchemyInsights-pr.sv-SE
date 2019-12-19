---
title: Felsöka befintlig bildskärm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738586"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="12de0-102">Felsöka en befintlig bildskärm</span><span class="sxs-lookup"><span data-stu-id="12de0-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="12de0-103">Prova dessa lösningar för att felsöka en bildskärm.</span><span class="sxs-lookup"><span data-stu-id="12de0-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="12de0-104">**Uppdatera bildskärmens display:**</span><span class="sxs-lookup"><span data-stu-id="12de0-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="12de0-105">Tryck på följande tangenter samtidigt: Windows-tangenten + Ctrl + Skift + B. Detta kommer att uppdatera kommunikationen med din grafikdrivrutin.</span><span class="sxs-lookup"><span data-stu-id="12de0-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="12de0-106">Dina bildskärmar kommer att blinka tillfälligt och komma tillbaka efter några sekunder.</span><span class="sxs-lookup"><span data-stu-id="12de0-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="12de0-107">**Felsöka bildskärms maskinvara:**</span><span class="sxs-lookup"><span data-stu-id="12de0-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="12de0-108">Koppla bort kabeln som ansluter datorn till bildskärmen och Anslut den igen.</span><span class="sxs-lookup"><span data-stu-id="12de0-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="12de0-109">Koppla bort alla icke-nödvändiga enheter från datorn (till exempel adaptrar eller dockor).</span><span class="sxs-lookup"><span data-stu-id="12de0-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="12de0-110">**Om du nyligen har installerat en uppdatering på datorn kan du återställa bildskärmsdrivrutinen:**</span><span class="sxs-lookup"><span data-stu-id="12de0-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="12de0-111">Välj **Start**, Skriv **Enhetshanteraren**och välj **Enhetshanteraren** i resultatet.</span><span class="sxs-lookup"><span data-stu-id="12de0-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="12de0-112">Expandera avsnittet **bildskärmskort** , högerklicka på bildskärmskortet, Ands Välj **Egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="12de0-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="12de0-113">Navigera till fliken **drivrutin** och välj **Återställ tillbaka drivrutin**.</span><span class="sxs-lookup"><span data-stu-id="12de0-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="12de0-114">Om detta inte är tillgängligt eller är nedtonat väljer du **Nej** i alternativen nedan för att gå vidare till nästa steg.</span><span class="sxs-lookup"><span data-stu-id="12de0-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="12de0-115">Du kan behöva starta om datorn innan ändringarna träder i kraft.</span><span class="sxs-lookup"><span data-stu-id="12de0-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="12de0-116">**Avinstallera och installera om bildskärmsdrivrutinen:**</span><span class="sxs-lookup"><span data-stu-id="12de0-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="12de0-117">Välj **Start**, Skriv **Enhetshanteraren**och välj **Enhetshanteraren** i resultatet.</span><span class="sxs-lookup"><span data-stu-id="12de0-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="12de0-118">Expandera avsnittet **bildskärmskort** , högerklicka på bildskärmskortet, Ands Välj **Avinstallera enhet**.</span><span class="sxs-lookup"><span data-stu-id="12de0-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="12de0-119">Markera rutan bredvid **ta bort drivrutinsprogramvaran för den här enheten** och välj **Avinstallera**.</span><span class="sxs-lookup"><span data-stu-id="12de0-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="12de0-120">Obs: du kan bli ombedd att starta om datorn i detta skede.</span><span class="sxs-lookup"><span data-stu-id="12de0-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="12de0-121">Se till att anteckna de återstående instruktionerna innan du startar om.</span><span class="sxs-lookup"><span data-stu-id="12de0-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="12de0-122">Öppna Enhetshanteraren igen.</span><span class="sxs-lookup"><span data-stu-id="12de0-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="12de0-123">Expandera avsnittet **bildskärmskort** , högerklicka på bildskärmskortet och välj **Uppdatera drivrutin**.</span><span class="sxs-lookup"><span data-stu-id="12de0-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="12de0-124">Välj **Sök automatiskt efter uppdatera drivrutinsprogramvara** och följ installationsanvisningarna.</span><span class="sxs-lookup"><span data-stu-id="12de0-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>