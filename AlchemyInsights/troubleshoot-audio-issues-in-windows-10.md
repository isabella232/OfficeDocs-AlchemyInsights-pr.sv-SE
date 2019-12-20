---
title: Felsöka ljudproblem i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796411"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="c76dd-102">Felsöka ljudproblem i Windows 10</span><span class="sxs-lookup"><span data-stu-id="c76dd-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="c76dd-103">**Kör felsökaren för ljud**</span><span class="sxs-lookup"><span data-stu-id="c76dd-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="c76dd-104">Ljudfelsökaren kanske kan åtgärda ljudproblemen automatiskt:</span><span class="sxs-lookup"><span data-stu-id="c76dd-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="c76dd-105">Välj **Start**, Skriv **Felsök**och välj sedan **Felsök** i listan med resultat.</span><span class="sxs-lookup"><span data-stu-id="c76dd-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="c76dd-106">Välj **spela upp ljud** > **Kör felsökaren**.</span><span class="sxs-lookup"><span data-stu-id="c76dd-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="c76dd-107">**Kontrollera kablar, volym, högtalare och hörlurar**</span><span class="sxs-lookup"><span data-stu-id="c76dd-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="c76dd-108">Kontrollera högtalar-och hörlurs anslutningarna för lösa kablar och kontrollera att de är anslutna till rätt uttag.</span><span class="sxs-lookup"><span data-stu-id="c76dd-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="c76dd-109">Kontrollera ström-och volymnivåerna och försök att vrida alla volymkontrollerna uppåt.</span><span class="sxs-lookup"><span data-stu-id="c76dd-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="c76dd-110">Vissa högtalare och appar har egna volymkontroller, och du kan behöva kontrollera dem alla för att se till att de är på rätt nivå.</span><span class="sxs-lookup"><span data-stu-id="c76dd-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="c76dd-111">Prova att ansluta med en annan USB-port.</span><span class="sxs-lookup"><span data-stu-id="c76dd-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="c76dd-112">**Anmärkning:** Kom ihåg att högtalarna kanske inte fungerar när hörlurarna är anslutna.</span><span class="sxs-lookup"><span data-stu-id="c76dd-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="c76dd-113">**Kontrollera Enhetshanteraren**</span><span class="sxs-lookup"><span data-stu-id="c76dd-113">**Check Device Manager**</span></span>

<span data-ttu-id="c76dd-114">Så här kontrollerar du att drivrutinerna är uppdaterade:</span><span class="sxs-lookup"><span data-stu-id="c76dd-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="c76dd-115">Välj **Start**, Skriv **Enhetshanteraren**och välj sedan **Enhetshanteraren** i listan med resultat.</span><span class="sxs-lookup"><span data-stu-id="c76dd-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="c76dd-116">Under **ljud-, video-och spelenheter**väljer du ljudkortet, öppnar det, väljer fliken **drivrutin** och väljer **Uppdatera drivrutin**.</span><span class="sxs-lookup"><span data-stu-id="c76dd-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="c76dd-117">**Anmärkning:** Om Windows inte hittar en ny drivrutin letar du efter en på enhetstillverkarens webbplats och följer deras instruktioner.</span><span class="sxs-lookup"><span data-stu-id="c76dd-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="c76dd-118">**Installera om drivrutinen**</span><span class="sxs-lookup"><span data-stu-id="c76dd-118">**Reinstall the driver**</span></span>

<span data-ttu-id="c76dd-119">Om du inte kan uppdatera via Enhetshanteraren eller hitta en ny drivrutin på tillverkarens webbplats provar du dessa steg:</span><span class="sxs-lookup"><span data-stu-id="c76dd-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="c76dd-120">Högerklicka på (eller håll ned) ljuddrivrutinen i Enhetshanteraren och välj **Avinstallera**.</span><span class="sxs-lookup"><span data-stu-id="c76dd-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="c76dd-121">Starta om enheten så försöker Windows att installera om drivrutinen.</span><span class="sxs-lookup"><span data-stu-id="c76dd-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="c76dd-122">Om ominstallation av drivrutinen inte fungerar provar du att använda den generiska ljuddrivrutinen som medföljer Windows.</span><span class="sxs-lookup"><span data-stu-id="c76dd-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="c76dd-123">I Enhetshanteraren, högerklicka (eller tryck och håll) ljuddrivrutinen > **Uppdatera drivrutinsprogramvara** > **Bläddra min dator för drivrutinsprogramvara** > **Låt mig välja från en lista över drivrutiner på min dator**, Välj **High Definition ljudenhet**, Välj **Nästa**, och följ instruktionerna för att installera den.</span><span class="sxs-lookup"><span data-stu-id="c76dd-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="c76dd-124">**Ställa in standardenhet**</span><span class="sxs-lookup"><span data-stu-id="c76dd-124">**Set the default device**</span></span>

<span data-ttu-id="c76dd-125">Om du ansluter till en ljudenhet med USB eller HDMI kan du behöva ställa in den enheten som standard:</span><span class="sxs-lookup"><span data-stu-id="c76dd-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="c76dd-126">Välj **Start**, Skriv **ljud**och välj sedan **ljud** eller **ändra systemljud** i listan med resultat.</span><span class="sxs-lookup"><span data-stu-id="c76dd-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="c76dd-127">Välj en enhet på fliken **uppspelning** , Välj **standard**och välj sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="c76dd-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

