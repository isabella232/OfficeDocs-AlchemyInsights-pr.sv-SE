---
title: Åtgärda problem med Bluetooth i Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730177"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="1ee79-102">Åtgärda problem med Bluetooth i Windows 10</span><span class="sxs-lookup"><span data-stu-id="1ee79-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="1ee79-103">Om Bluetooth-ikonen saknas eller om det inte går att aktivera eller inaktivera Bluetooth kan du köra fel sökaren för Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="1ee79-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="1ee79-104">[Öppna fel söknings inställningar](ms-settings:troubleshoot), klicka på **Bluetooth** under **hitta och åtgärda andra problem**klickar **du på kör fel sökaren**.</span><span class="sxs-lookup"><span data-stu-id="1ee79-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="1ee79-105">Om du inte ser Bluetooth-ikonen men Bluetooth visas i enhets hanteraren:</span><span class="sxs-lookup"><span data-stu-id="1ee79-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="1ee79-106">Klicka på **Bluetooth**i enhets hanteraren.</span><span class="sxs-lookup"><span data-stu-id="1ee79-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="1ee79-107">Tryck och håll ned (eller högerklicka på) namnet på Bluetooth-kortet och klicka på **Avinstallera enhet**.</span><span class="sxs-lookup"><span data-stu-id="1ee79-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="1ee79-108">Stäng av Windows-enheten, vänta några sekunder och slå sedan på den igen.</span><span class="sxs-lookup"><span data-stu-id="1ee79-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="1ee79-109">Windows försöker installera om driv rutinen.</span><span class="sxs-lookup"><span data-stu-id="1ee79-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="1ee79-110">Om du nyligen har installerat uppdateringar för Windows 10 eller uppgraderat till Windows 10 kan det vara bra att söka efter driv rutins uppdateringar:</span><span class="sxs-lookup"><span data-stu-id="1ee79-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="1ee79-111">Klicka på **Bluetooth**i enhets hanteraren och klicka sedan på namnet på Bluetooth-kortet (som kan innehålla ordet "Radio").</span><span class="sxs-lookup"><span data-stu-id="1ee79-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="1ee79-112">Håll ned (eller högerklicka) på Bluetooth-kortet och klicka sedan på Uppdatera Sök efter **driv rutin**  >  **automatiskt för uppdaterade driv rutiner**.</span><span class="sxs-lookup"><span data-stu-id="1ee79-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="1ee79-113">Följ stegen och klicka sedan på **Stäng**.</span><span class="sxs-lookup"><span data-stu-id="1ee79-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="1ee79-114">Om Windows inte hittar en ny Bluetooth-drivrutin kan du besöka PC-tillverkarens webbplats och ladda ner den senaste Bluetooth-drivrutinen därifrån.</span><span class="sxs-lookup"><span data-stu-id="1ee79-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="1ee79-115">När du har laddat ner det klickar du på **Uppdatera driv rutin**  >  **Bläddra på datorn efter driv rutiner**  >  **Bläddra** efter den plats där drivrutinsfilerna lagras > **OK**  >  **Nästa**och följer anvisningarna för att installera.</span><span class="sxs-lookup"><span data-stu-id="1ee79-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="1ee79-116">När du har installerat den uppdaterade driv rutinen startar du om datorn och kontrollerar sedan om det löser anslutnings problemet.</span><span class="sxs-lookup"><span data-stu-id="1ee79-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="1ee79-117">Mer information om hur du felsöker Bluetooth-problem finns i artikeln om att [åtgärda Bluetooth-problem i Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="1ee79-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
