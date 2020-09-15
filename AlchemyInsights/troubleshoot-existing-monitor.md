---
title: Felsöka befintlig bildskärm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690729"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="ebbda-102">Felsöka en befintlig bildskärm</span><span class="sxs-lookup"><span data-stu-id="ebbda-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="ebbda-103">Prova de här lösningarna för att felsöka en bildskärm.</span><span class="sxs-lookup"><span data-stu-id="ebbda-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="ebbda-104">**Uppdatera bildskärmens skärm:**</span><span class="sxs-lookup"><span data-stu-id="ebbda-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="ebbda-105">Tryck på följande tangenter samtidigt: Windows-tangenten + Ctrl + Skift + B. Då uppdateras kommunikationen med grafik driv rutinen.</span><span class="sxs-lookup"><span data-stu-id="ebbda-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="ebbda-106">Dina skärmar blinkar tillfälligt och kommer tillbaka efter några sekunder.</span><span class="sxs-lookup"><span data-stu-id="ebbda-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="ebbda-107">**Felsöka skärm maskin vara:**</span><span class="sxs-lookup"><span data-stu-id="ebbda-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="ebbda-108">Koppla bort kabeln som ansluter datorn till din bildskärm och koppla in den igen.</span><span class="sxs-lookup"><span data-stu-id="ebbda-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="ebbda-109">Koppla bort alla icke-väsentliga enheter från datorn (till exempel adaptrar eller dock).</span><span class="sxs-lookup"><span data-stu-id="ebbda-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="ebbda-110">**Om du nyligen har installerat en uppdatering på datorn kan du återställa bildskärmens driv rutinen:**</span><span class="sxs-lookup"><span data-stu-id="ebbda-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="ebbda-111">Välj **Start**, Skriv **enhets hanteraren**och välj **enhets hanteraren** från resultaten.</span><span class="sxs-lookup"><span data-stu-id="ebbda-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="ebbda-112">Expandera avsnittet **bildskärms kort** , högerklicka på bildskärms kortet, Ands Välj **Egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="ebbda-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="ebbda-113">Gå till fliken **driv rutin** och välj **Återställ driv rutin**.</span><span class="sxs-lookup"><span data-stu-id="ebbda-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="ebbda-114">OBS! om det inte är tillgängligt eller är nedtonat väljer du **Nej** från alternativen nedan för att gå till nästa steg.</span><span class="sxs-lookup"><span data-stu-id="ebbda-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="ebbda-115">Du kan behöva starta om datorn innan ändringarna börjar gälla.</span><span class="sxs-lookup"><span data-stu-id="ebbda-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="ebbda-116">**Avinstallera och installera om bildskärms driv rutinen:**</span><span class="sxs-lookup"><span data-stu-id="ebbda-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="ebbda-117">Välj **Start**, Skriv **enhets hanteraren**och välj **enhets hanteraren** från resultaten.</span><span class="sxs-lookup"><span data-stu-id="ebbda-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="ebbda-118">Expandera avsnittet **bildskärms kort** , högerklicka på bildskärms kortet, Ands Välj **Avinstallera enhet**.</span><span class="sxs-lookup"><span data-stu-id="ebbda-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="ebbda-119">Markera rutan bredvid **ta bort driv rutinen för den här enheten** och välj **Avinstallera**.</span><span class="sxs-lookup"><span data-stu-id="ebbda-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="ebbda-120">Obs! Du kan uppmanas att starta om datorn i den här fasen.</span><span class="sxs-lookup"><span data-stu-id="ebbda-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="ebbda-121">Skriv ned de återstående anvisningarna innan du startar om.</span><span class="sxs-lookup"><span data-stu-id="ebbda-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="ebbda-122">Öppna enhets hanteraren igen.</span><span class="sxs-lookup"><span data-stu-id="ebbda-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="ebbda-123">Expandera avsnittet **bildskärms kort** , högerklicka på bildskärms kortet och välj **Uppdatera driv rutin**.</span><span class="sxs-lookup"><span data-stu-id="ebbda-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="ebbda-124">Välj **Sök automatiskt för uppdatera driv rutiner** och följ installations anvisningarna.</span><span class="sxs-lookup"><span data-stu-id="ebbda-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>