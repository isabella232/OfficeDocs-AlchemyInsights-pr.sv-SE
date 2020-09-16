---
title: Felsöka ljud problem i Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750361"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="08036-102">Felsöka ljud problem i Windows 10</span><span class="sxs-lookup"><span data-stu-id="08036-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="08036-103">**Köra fel sökaren för ljud**</span><span class="sxs-lookup"><span data-stu-id="08036-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="08036-104">Öppna [fel söknings inställningar](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="08036-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="08036-105">Välj **spela upp ljud**  >  **kör fel sökaren**.</span><span class="sxs-lookup"><span data-stu-id="08036-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="08036-106">**Ange standardenhet**</span><span class="sxs-lookup"><span data-stu-id="08036-106">**Set the default device**</span></span>

<span data-ttu-id="08036-107">Om du ansluter till en ljuden het med USB eller HDMI kan du behöva ange enheten som standard:</span><span class="sxs-lookup"><span data-stu-id="08036-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="08036-108">Öppna **Start**  >  **ljud**och välj sedan **ljud** eller **ändra system ljud** i resultat listan.</span><span class="sxs-lookup"><span data-stu-id="08036-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="08036-109">Välj en enhet på fliken **uppspelning** och välj **Ange standard**och sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="08036-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="08036-110">**Kontrol lera kablar, volym, högtalare och hörlurar**</span><span class="sxs-lookup"><span data-stu-id="08036-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="08036-111">Kontrol lera att du har kablar och hörlurs samtal och se till att de är anslutna till rätt uttag.</span><span class="sxs-lookup"><span data-stu-id="08036-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="08036-112">Kontrol lera energi-och volym nivåerna och prova att aktivera alla volym kontroller.</span><span class="sxs-lookup"><span data-stu-id="08036-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="08036-113">Vissa högtalare och appar har sina egna volym kontroller; Du kanske måste kontrol lera dem så att de är på rätt nivå.</span><span class="sxs-lookup"><span data-stu-id="08036-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="08036-114">Prova att ansluta med en annan USB-port.</span><span class="sxs-lookup"><span data-stu-id="08036-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="08036-115">**Obs!** kom ihåg att dina högtalare kanske inte fungerar när hörlurarna ansluts.</span><span class="sxs-lookup"><span data-stu-id="08036-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="08036-116">**Kontrol lera enhets hanteraren**</span><span class="sxs-lookup"><span data-stu-id="08036-116">**Check Device Manager**</span></span>

<span data-ttu-id="08036-117">Så här kontrollerar du att driv rutinerna är uppdaterade:</span><span class="sxs-lookup"><span data-stu-id="08036-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="08036-118">Välj **Start**, Skriv **enhets hanteraren**och välj sedan **enhets hanteraren** i resultat listan.</span><span class="sxs-lookup"><span data-stu-id="08036-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="08036-119">Välj ljud kortet under **ljud-, video-och spel enheter**, öppna det, Välj fliken **driv rutin** och välj **Uppdatera driv rutin**.</span><span class="sxs-lookup"><span data-stu-id="08036-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="08036-120">**Obs!** om Windows inte hittar en ny driv rutin kan du leta efter en på tillverkarens webbplats och följa deras instruktioner.</span><span class="sxs-lookup"><span data-stu-id="08036-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="08036-121">**Installera om driv rutinen**</span><span class="sxs-lookup"><span data-stu-id="08036-121">**Reinstall the driver**</span></span>

<span data-ttu-id="08036-122">Om du inte kan uppdatera via enhets hanteraren eller hitta en ny driv rutin på tillverkarens webbplats kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="08036-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="08036-123">Högerklicka på (eller håll ned) ljud driv rutinen i enhets hanteraren och välj **Avinstallera**.</span><span class="sxs-lookup"><span data-stu-id="08036-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="08036-124">Starta om enheten så försöker Windows installera om driv rutinen.</span><span class="sxs-lookup"><span data-stu-id="08036-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="08036-125">Om det inte fungerar att installera om driv rutinen kan du försöka använda den allmänna ljud driv rutinen som medföljer Windows.</span><span class="sxs-lookup"><span data-stu-id="08036-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="08036-126">I enhets hanteraren högerklickar du på (eller trycker på och håller ned) ljud driv rutinen > **Uppdatera driv**rutin  >  **Bläddra på den här datorn efter driv**rutiner kan du välja  >  **från en lista på**driv rutinen på datorn, välja HD- **ljudenhet**, välja **Nästa**och följa anvisningarna för att installera den.</span><span class="sxs-lookup"><span data-stu-id="08036-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
