---
title: Startinställningar i Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828170"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="270e3-102">Startinställningar i Windows 10</span><span class="sxs-lookup"><span data-stu-id="270e3-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="270e3-103">**Ändra vilka appar som körs automatiskt vid start**</span><span class="sxs-lookup"><span data-stu-id="270e3-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="270e3-104">Gå till [Inställningar > Program > Start](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="270e3-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="270e3-105">Kontrollera att alla appar som du vill köra vid start **är** på .</span><span class="sxs-lookup"><span data-stu-id="270e3-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="270e3-106">**Lägga till ett program som ska köras automatiskt vid start**</span><span class="sxs-lookup"><span data-stu-id="270e3-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="270e3-107">Klicka eller tryck **på Start** och leta reda på programmet du vill köra vid start.</span><span class="sxs-lookup"><span data-stu-id="270e3-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="270e3-108">Högerklicka på programmet, klicka på **Mer och** klicka sedan på **Öppna filplats**.</span><span class="sxs-lookup"><span data-stu-id="270e3-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="270e3-109">Då öppnas den plats där genvägen till programmet sparas.</span><span class="sxs-lookup"><span data-stu-id="270e3-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="270e3-110">Om det inte finns något alternativ för Öppna filplats betyder det att programmet inte kan köras vid start.</span><span class="sxs-lookup"><span data-stu-id="270e3-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="270e3-111">Med filplatsen öppen trycker du på **Windows-tangenten + R,** skriver **shell:startup** och klickar sedan på **OK.**</span><span class="sxs-lookup"><span data-stu-id="270e3-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="270e3-112">Då öppnas mappen Autostart.</span><span class="sxs-lookup"><span data-stu-id="270e3-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="270e3-113">Kopiera och klistra in genvägen till programmet från filens plats i startmappen.</span><span class="sxs-lookup"><span data-stu-id="270e3-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="270e3-114">**Avancerade startalternativ (inklusive felsäkert läge, UEFI-inställningar och start från en annan enhet)**</span><span class="sxs-lookup"><span data-stu-id="270e3-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="270e3-115">Spara ditt arbete och stäng alla öppna dokument eftersom de här stegen startar om datorn.</span><span class="sxs-lookup"><span data-stu-id="270e3-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="270e3-116">Gå till [Inställningar > Uppdatering & Säkerhetsinställningar > Återställning](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="270e3-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="270e3-117">Klicka **på Starta om** nu under Avancerad **start.**</span><span class="sxs-lookup"><span data-stu-id="270e3-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="270e3-118">När datorn startats om till skärmen Välj ett alternativ:</span><span class="sxs-lookup"><span data-stu-id="270e3-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="270e3-119">Om du vill starta från en enhet som en USB-enhet klickar du **på Använd en enhet**.</span><span class="sxs-lookup"><span data-stu-id="270e3-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="270e3-120">Om du vill ange UEFI-inställningarna (kallas ibland FÖR TIDSKONFIGURATION) klickar du **> Avancerade alternativ > inbyggd UEFI-inställning.**</span><span class="sxs-lookup"><span data-stu-id="270e3-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="270e3-121">Om du vill öppna felsäkert läge eller ändra avancerade startinställningar klickar du > På avancerade **> inställningar** och sedan på Starta **om**.</span><span class="sxs-lookup"><span data-stu-id="270e3-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="270e3-122">Du kan bli ombedd att ange din [BitLocker-återställningsnyckel](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="270e3-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="270e3-123">När datorn har startats om igen klickar du på den startinställning du vill använda.</span><span class="sxs-lookup"><span data-stu-id="270e3-123">After your PC restarts again, click the startup setting you want to use.</span></span>