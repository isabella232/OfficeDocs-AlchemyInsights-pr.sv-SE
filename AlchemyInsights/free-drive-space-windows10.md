---
title: Frigöra diskutrymme i Windows 10
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037950"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="46901-102">Frigöra diskutrymme i Windows 10</span><span class="sxs-lookup"><span data-stu-id="46901-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="46901-103">Här är två alternativ för att frigöra diskutrymme i Windows:</span><span class="sxs-lookup"><span data-stu-id="46901-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="46901-104">Frigör diskutrymme i Windows 10.</span><span class="sxs-lookup"><span data-stu-id="46901-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="46901-105">Frigör utrymme för Windows 10-uppdateringar med extern lagringsenhet.</span><span class="sxs-lookup"><span data-stu-id="46901-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="46901-106">Om du fortfarande har låg diskutrymme efter att ha använt Diskrensning är det möjligt att Temp-mappen snabbt fylls upp med programfiler (.appx) som används av Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="46901-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="46901-107">Lös problemet genom att återställa Store, rensa Store-cachen och sedan köra Felsökaren för Windows Update.</span><span class="sxs-lookup"><span data-stu-id="46901-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="46901-108">Se till att Microsoft Store är stängt innan du fortsätter med de här stegen.</span><span class="sxs-lookup"><span data-stu-id="46901-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="46901-109">**Steg 1: Återställ Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="46901-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="46901-110">**Obs!** Då tas appdata på enheten bort permanent, inklusive dina inställningar och inloggningsuppgifter.</span><span class="sxs-lookup"><span data-stu-id="46901-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="46901-111">Välj **Starta**  >  **inställningar**  >  **Appar**  >  **& funktioner**.</span><span class="sxs-lookup"><span data-stu-id="46901-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="46901-112">Leta reda på och välj Microsoft Store i listan med appar.</span><span class="sxs-lookup"><span data-stu-id="46901-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="46901-113">Välj **Avancerade alternativ**.</span><span class="sxs-lookup"><span data-stu-id="46901-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="46901-114">Rulla nedåt och välj **Återställ** och sedan **Bekräfta återställning.**</span><span class="sxs-lookup"><span data-stu-id="46901-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="46901-115">**Steg 2: Rensa Microsoft Store-cachen**</span><span class="sxs-lookup"><span data-stu-id="46901-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="46901-116">Tryck på Windows-tangenten + R för att öppna dialogrutan Kör.</span><span class="sxs-lookup"><span data-stu-id="46901-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="46901-117">Skriv wsreset.exe och välj **OK**.</span><span class="sxs-lookup"><span data-stu-id="46901-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="46901-118">Ett tomt kommandotolkfönster öppnas.</span><span class="sxs-lookup"><span data-stu-id="46901-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="46901-119">Efter ungefär 10 sekunder stängs fönstret och Store öppnas automatiskt.</span><span class="sxs-lookup"><span data-stu-id="46901-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="46901-120">**Steg 3: Återställ Windows Update**</span><span class="sxs-lookup"><span data-stu-id="46901-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="46901-121">Välj **Starta**  >  **inställningar**  >  **Uppdatering &**  >  **säkerhetsfelsök**.</span><span class="sxs-lookup"><span data-stu-id="46901-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="46901-122">Rulla nedåt och **välj Windows Update** i listan och välj Kör **felsökaren**.</span><span class="sxs-lookup"><span data-stu-id="46901-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="46901-123">Starta om datorn och kontrollera om du fortfarande upplever problemet.</span><span class="sxs-lookup"><span data-stu-id="46901-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

