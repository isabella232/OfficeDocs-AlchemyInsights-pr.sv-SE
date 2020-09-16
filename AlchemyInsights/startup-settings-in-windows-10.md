---
title: Start Inställningar i Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751153"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="d0d6e-102">Start Inställningar i Windows 10</span><span class="sxs-lookup"><span data-stu-id="d0d6e-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="d0d6e-103">**Ändra vilka appar som körs automatiskt vid start**</span><span class="sxs-lookup"><span data-stu-id="d0d6e-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="d0d6e-104">Gå till [inställningar > appar > start](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="d0d6e-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="d0d6e-105">Se till att alla program du vill köra vid **Start är aktiverat.**</span><span class="sxs-lookup"><span data-stu-id="d0d6e-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="d0d6e-106">**Lägga till ett program som ska köras automatiskt vid start**</span><span class="sxs-lookup"><span data-stu-id="d0d6e-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="d0d6e-107">Klicka eller tryck på **Start** och leta reda på det program du vill köra vid start.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="d0d6e-108">Högerklicka på appen, klicka på **mer**och sedan på **Öppna fil Sök väg**.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="d0d6e-109">Då öppnas platsen där genvägen till programmet har sparats.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="d0d6e-110">Om det inte finns något alternativ för att öppna fil Sök vägen innebär det att appen inte kan köras vid start.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="d0d6e-111">Öppna fil platsen och tryck på Windows- **tangenten + R**, Skriv **Shell: Start**och klicka sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="d0d6e-112">Då öppnas startmappen.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="d0d6e-113">Kopiera och klistra in genvägen till appen från fil platsen till mappen Start.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="d0d6e-114">**Avancerade start alternativ (inklusive fel säkert läge, UEFI-inställningar och start från en annan enhet)**</span><span class="sxs-lookup"><span data-stu-id="d0d6e-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="d0d6e-115">Spara ditt arbete och Stäng alla öppna dokument eftersom de här anvisningarna startar om datorn.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="d0d6e-116">Gå till [inställningar > uppdatering & säkerhets > återställning](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="d0d6e-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="d0d6e-117">Klicka på **starta om nu**under **Avancerad start**.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="d0d6e-118">När du har startat om datorn på skärmen Välj ett alternativ:</span><span class="sxs-lookup"><span data-stu-id="d0d6e-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="d0d6e-119">Om du vill starta från en enhet som en USB-enhet klickar du på **Använd en enhet**.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="d0d6e-120">Om du vill ange UEFI-inställningar (kallas ibland BIOS-konfiguration) klickar du på **felsöka > avancerade alternativ > UEFI-inställningar**.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="d0d6e-121">Om du vill öppna fel säkert läge eller ändra avancerade Start Inställningar klickar du på **felsöka > avancerade alternativ > Start Inställningar**och klickar sedan på **starta om**.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="d0d6e-122">Du kan uppmanas att ange din [återställnings nyckel för BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="d0d6e-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="d0d6e-123">När datorn har startat om klickar du på den Start inställning du vill använda.</span><span class="sxs-lookup"><span data-stu-id="d0d6e-123">After your PC restarts again, click the startup setting you want to use.</span></span>