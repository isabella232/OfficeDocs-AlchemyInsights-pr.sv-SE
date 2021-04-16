---
title: Åtgärda Bluetooth-problem i Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812950"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="64fde-102">Åtgärda Bluetooth-problem i Windows 10</span><span class="sxs-lookup"><span data-stu-id="64fde-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="64fde-103">Om Bluetooth-ikonen saknas eller om Bluetooth inte kan aktiveras eller inaktiveras kan du köra Bluetooth-felsökaren.</span><span class="sxs-lookup"><span data-stu-id="64fde-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="64fde-104">[Öppna felsökningsinställningarna](ms-settings:troubleshoot), klicka på **Bluetooth** under **Hitta och åtgärda andra problem** och klicka på Kör **felsökaren.**</span><span class="sxs-lookup"><span data-stu-id="64fde-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="64fde-105">Om Bluetooth-ikonen inte visas, men Bluetooth visas i Enhetshanteraren:</span><span class="sxs-lookup"><span data-stu-id="64fde-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="64fde-106">Klicka på Bluetooth i **Enhetshanteraren.**</span><span class="sxs-lookup"><span data-stu-id="64fde-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="64fde-107">Håll ned (eller högerklicka på) Bluetooth-adapterns namn och klicka på **Avinstallera enhet**.</span><span class="sxs-lookup"><span data-stu-id="64fde-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="64fde-108">Stäng av Windows-enheten, vänta några sekunder och aktivera den sedan igen.</span><span class="sxs-lookup"><span data-stu-id="64fde-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="64fde-109">Windows försöker installera om drivrutinen.</span><span class="sxs-lookup"><span data-stu-id="64fde-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="64fde-110">Om du nyligen har installerat Windows 10-uppdateringar eller uppgraderat till Windows 10 kanske du vill söka efter drivrutinsuppdateringar:</span><span class="sxs-lookup"><span data-stu-id="64fde-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="64fde-111">I Enhetshanteraren klickar du **på Bluetooth** och sedan på namnet på Bluetooth-adaptern (vilket kan inkludera ordet "radio").</span><span class="sxs-lookup"><span data-stu-id="64fde-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="64fde-112">Håll ned (eller högerklicka på) Bluetooth-adaptern och klicka sedan på **Uppdatera**  >  **drivrutinssökning automatiskt för uppdaterad drivrutinsprogramvara.**</span><span class="sxs-lookup"><span data-stu-id="64fde-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="64fde-113">Följ anvisningarna och klicka sedan på **Stäng.**</span><span class="sxs-lookup"><span data-stu-id="64fde-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="64fde-114">Om Windows inte kan hitta en ny Bluetooth-drivrutin går du till datortillverkarens webbplats och laddar ned den senaste Bluetooth-drivrutinen därifrån.</span><span class="sxs-lookup"><span data-stu-id="64fde-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="64fde-115">När du har laddat ned den klickar du på Uppdatera drivrutin Bläddra i datorn efter drivrutinsprogramvara Bläddra efter den plats där drivrutinsfilerna lagras > OK Nästa och följ anvisningarna  >    >   för   >  att installera.</span><span class="sxs-lookup"><span data-stu-id="64fde-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="64fde-116">När du har installerat den uppdaterade drivrutinen startar du om datorn och kontrollerar om det löser problemet.</span><span class="sxs-lookup"><span data-stu-id="64fde-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="64fde-117">Mer information om hur du felsöker Bluetooth-problem finns i den fullständiga artikeln Åtgärda [Bluetooth-problem i Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="64fde-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
