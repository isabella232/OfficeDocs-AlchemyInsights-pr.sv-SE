---
title: Felsöka ljudproblem i Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833309"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="84b53-102">Felsöka ljudproblem i Windows 10</span><span class="sxs-lookup"><span data-stu-id="84b53-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="84b53-103">**Köra felsökaren för ljud**</span><span class="sxs-lookup"><span data-stu-id="84b53-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="84b53-104">Öppna [felsökningsinställningarna.](ms-settings:troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="84b53-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="84b53-105">Välj **Ljuduppspelning**  >  **Kör felsökaren**.</span><span class="sxs-lookup"><span data-stu-id="84b53-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="84b53-106">**Ange standardenhet**</span><span class="sxs-lookup"><span data-stu-id="84b53-106">**Set the default device**</span></span>

<span data-ttu-id="84b53-107">Om du ansluter till en ljudenhet med USB eller HDMI kan du behöva ange den enheten som standardenhet:</span><span class="sxs-lookup"><span data-stu-id="84b53-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="84b53-108">Öppna **Starta**  >  **ljud** och välj sedan **Ljud eller** Ändra **systemljud** i listan med resultat.</span><span class="sxs-lookup"><span data-stu-id="84b53-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="84b53-109">Välj **en enhet** på fliken Uppspelning, välj **Ange standard** och välj sedan **OK.**</span><span class="sxs-lookup"><span data-stu-id="84b53-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="84b53-110">**Kontrollera kablar, volym, högtalare och hörlurar**</span><span class="sxs-lookup"><span data-stu-id="84b53-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="84b53-111">Kontrollera att alla kablar är korrekt anslutna i högtalarna och hörlurarna och att de är anslutna till rätt uttag.</span><span class="sxs-lookup"><span data-stu-id="84b53-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="84b53-112">Kontrollera ström och volym, och prova att vrida upp alla volymkontroller.</span><span class="sxs-lookup"><span data-stu-id="84b53-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="84b53-113">Vissa högtalare och appar har egna volymkontroller. du kanske måste kontrollera alla för att säkerställa att de är på rätt nivåer.</span><span class="sxs-lookup"><span data-stu-id="84b53-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="84b53-114">Prova att ansluta via en annan USB-port.</span><span class="sxs-lookup"><span data-stu-id="84b53-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="84b53-115">**Obs!** Kom ihåg att högtalarna kanske inte fungerar när hörlurar är inkopplade.</span><span class="sxs-lookup"><span data-stu-id="84b53-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="84b53-116">**Kontrollera Enhetshanteraren**</span><span class="sxs-lookup"><span data-stu-id="84b53-116">**Check Device Manager**</span></span>

<span data-ttu-id="84b53-117">Så här kontrollerar du att drivrutinerna är uppdaterade:</span><span class="sxs-lookup"><span data-stu-id="84b53-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="84b53-118">Välj **Start**, **skriv Enhetshanteraren** och välj **sedan Enhetshanteraren** i listan med resultat.</span><span class="sxs-lookup"><span data-stu-id="84b53-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="84b53-119">Under **Ljud-, video- och spelenheter** väljer du ditt ljudkort, öppnar det, väljer fliken **Drivrutin** och väljer Uppdatera **drivrutin.**</span><span class="sxs-lookup"><span data-stu-id="84b53-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="84b53-120">**Obs!** Om Windows inte hittar en ny drivrutin letar du upp en på enhetstillverkarens webbplats och följer deras anvisningar.</span><span class="sxs-lookup"><span data-stu-id="84b53-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="84b53-121">**Installera om drivrutinen**</span><span class="sxs-lookup"><span data-stu-id="84b53-121">**Reinstall the driver**</span></span>

<span data-ttu-id="84b53-122">Om du inte kan uppdatera via Enhetshanteraren eller hitta en ny drivrutin på tillverkarens webbplats kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="84b53-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="84b53-123">I Enhetshanteraren högerklickar du på (eller håller ned) ljuddrivrutinen och väljer **Avinstallera.**</span><span class="sxs-lookup"><span data-stu-id="84b53-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="84b53-124">Starta om enheten så försöker Windows installera om drivrutinen.</span><span class="sxs-lookup"><span data-stu-id="84b53-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="84b53-125">Om det inte fungerar att installera om drivrutinen kan du prova att använda den allmänna ljuddrivrutinen som medföljer Windows.</span><span class="sxs-lookup"><span data-stu-id="84b53-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="84b53-126">I Enhetshanteraren högerklickar du på (eller håller ned) din ljuddrivrutin > Uppdatera drivrutinsprogramvara Bläddra i datorn efter drivrutinsprogramvara Låt mig välja från en lista med drivrutiner på datorn , välj High Definition Audio Device , välj Nästa och följ anvisningarna för att installera  >    >  den.  </span><span class="sxs-lookup"><span data-stu-id="84b53-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
