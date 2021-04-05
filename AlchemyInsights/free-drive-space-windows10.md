---
title: Frigör diskutrymme i Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505374"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="e0f90-102">Frigör diskutrymme i Windows 10</span><span class="sxs-lookup"><span data-stu-id="e0f90-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="e0f90-103">Här är två alternativ för att frigöra diskutrymme i Windows:</span><span class="sxs-lookup"><span data-stu-id="e0f90-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="e0f90-104">Frigör diskutrymme i Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e0f90-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="e0f90-105">Frigör utrymme för Windows 10-uppdateringar med en extern lagringsenhet.</span><span class="sxs-lookup"><span data-stu-id="e0f90-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="e0f90-106">Om du fortfarande har låg diskutrymme efter att du har använt Diskrensning är det möjligt att Temp-mappen snabbt fylls på med programfiler (.appx) som används i Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="e0f90-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="e0f90-107">Lös problemet genom att återställa Store, rensa Store-cachen och kör sedan felsökaren för Windows Update.</span><span class="sxs-lookup"><span data-stu-id="e0f90-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="e0f90-108">Kontrollera att Microsoft Store är stängt innan du fortsätter med de här stegen.</span><span class="sxs-lookup"><span data-stu-id="e0f90-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="e0f90-109">**Steg 1: Återställ Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="e0f90-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="e0f90-110">**Obs** Detta tar bort appdata på enheten permanent, inklusive dina inställningar och inloggningsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="e0f90-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="e0f90-111">Välj **Start** > **Inställningar** > **Appar** > **Appar och funktioner**.</span><span class="sxs-lookup"><span data-stu-id="e0f90-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="e0f90-112">Leta reda på och välj Microsoft Store i listan med program.</span><span class="sxs-lookup"><span data-stu-id="e0f90-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="e0f90-113">Välj **Avancerade alternativ**.</span><span class="sxs-lookup"><span data-stu-id="e0f90-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="e0f90-114">Rulla nedåt och välj **Återställa** och välj sedan **Bekräfta återställa**.</span><span class="sxs-lookup"><span data-stu-id="e0f90-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="e0f90-115">**Steg 2: Rensa Microsoft Store-cachen**</span><span class="sxs-lookup"><span data-stu-id="e0f90-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="e0f90-116">Tryck på Windows-tangenten+R för att öppna dialogrutan Kör.</span><span class="sxs-lookup"><span data-stu-id="e0f90-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="e0f90-117">Skriv wsreset.exe och välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="e0f90-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="e0f90-118">Ett tomt Kommandotolkens fönster öppnas.</span><span class="sxs-lookup"><span data-stu-id="e0f90-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="e0f90-119">Efter ungefär 10 sekunder stängs fönstret och Store öppnas automatiskt.</span><span class="sxs-lookup"><span data-stu-id="e0f90-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="e0f90-120">**Steg 3: Återställa Windows Update**</span><span class="sxs-lookup"><span data-stu-id="e0f90-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="e0f90-121">Välj **Start** > **Inställningar** > **Uppdatera och Säkerhet** > **Felsöka**.</span><span class="sxs-lookup"><span data-stu-id="e0f90-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="e0f90-122">Rulla nedåt och välj **Windows Update** i listan och välj **Kör felsökaren**.</span><span class="sxs-lookup"><span data-stu-id="e0f90-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="e0f90-123">Starta om datorn och kontrollera om du fortfarande har det här problemet.</span><span class="sxs-lookup"><span data-stu-id="e0f90-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

