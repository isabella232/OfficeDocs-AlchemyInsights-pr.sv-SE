---
title: Använd alternativet för att låsa upp finger i Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795262"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="00f35-102">Använd alternativet för att låsa upp finger i Windows 10</span><span class="sxs-lookup"><span data-stu-id="00f35-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="00f35-103">**Aktivera finger avtryck för Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="00f35-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="00f35-104">För att låsa upp Windows 10 med ditt finger avtryck måste du konfigurera Windows Hello-finger avtryck genom att lägga till (och låta Windows lära sig känna igen) minst ett finger.</span><span class="sxs-lookup"><span data-stu-id="00f35-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="00f35-105">Gå till **inställningar > konton > inloggnings alternativ** (eller klicka [här](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="00f35-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="00f35-106">Tillgängliga inloggnings alternativ visas.</span><span class="sxs-lookup"><span data-stu-id="00f35-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="00f35-107">Ett exempel:</span><span class="sxs-lookup"><span data-stu-id="00f35-107">For example:</span></span>

    ![Inloggnings alternativ.](media/sign-in-options.png)

2. <span data-ttu-id="00f35-109">Klicka eller tryck på **Windows Hello-finger avtryck**och sedan på **Konfigurera**.</span><span class="sxs-lookup"><span data-stu-id="00f35-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="00f35-110">I fönstret Windows Hello-inställningar klickar du på **komma igång**.</span><span class="sxs-lookup"><span data-stu-id="00f35-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="00f35-111">Finger avtrycks sensorn aktive ras och du uppmanas att placera fingret på sensorn:</span><span class="sxs-lookup"><span data-stu-id="00f35-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Finger avtryck.](media/fingerprint-sensor.png)

3. <span data-ttu-id="00f35-113">Följ instruktionerna som ber dig att upprepade gånger kontrol lera ditt finger.</span><span class="sxs-lookup"><span data-stu-id="00f35-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="00f35-114">När det är klart kan du välja att lägga till andra fingrar som du kan använda för inloggning.</span><span class="sxs-lookup"><span data-stu-id="00f35-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="00f35-115">Nästa gång du loggar in i Windows 10 kan du välja att använda ditt finger avtryck för att göra det.</span><span class="sxs-lookup"><span data-stu-id="00f35-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="00f35-116">**Windows Hello-finger avtryck är inte tillgängligt som inloggnings alternativ**</span><span class="sxs-lookup"><span data-stu-id="00f35-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="00f35-117">Om Windows Hello-finger avtryck inte visas som ett alternativ i **inloggnings alternativ**innebär det att Windows inte känner till vilken finger avtrycks läsare/skanner som är ansluten till datorn eller att en system princip hindrar dess användning (om till exempel din dator hanteras av din arbets plats).</span><span class="sxs-lookup"><span data-stu-id="00f35-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="00f35-118">Så här felsöker du:</span><span class="sxs-lookup"><span data-stu-id="00f35-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="00f35-119">Välj **Start** -knappen i aktivitets fältet och Sök efter **enhets hanteraren**.</span><span class="sxs-lookup"><span data-stu-id="00f35-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="00f35-120">Klicka eller tryck för att öppna **enhets hanteraren**.</span><span class="sxs-lookup"><span data-stu-id="00f35-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="00f35-121">I enhets hanteraren expanderar du bio metriska enheter genom att klicka på dess gränssnitt.</span><span class="sxs-lookup"><span data-stu-id="00f35-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Bio metriska enheter.](media/biometric-devices.png)

4. <span data-ttu-id="00f35-123">Din finger avtrycks läsare ska visas som en bio Metrisk enhet, till exempel Synaptics WBDI-skanner:</span><span class="sxs-lookup"><span data-stu-id="00f35-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Bio metriska enheter.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="00f35-125">Om din finger avtrycks läsare inte visas och skannern är inbyggd i datorn går du till tillverkarens webbplats.</span><span class="sxs-lookup"><span data-stu-id="00f35-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="00f35-126">I avsnittet teknisk support för dator modellen söker du efter en Windows 10-drivrutin för en skanner som du kan installera.</span><span class="sxs-lookup"><span data-stu-id="00f35-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="00f35-127">Om skannern är avgränsad från datorn (ansluten via USB) går du till skanner tillverkarens webbplats för att hitta och installera Windows 10-enhets driv rutiner för den skanner modell du har.</span><span class="sxs-lookup"><span data-stu-id="00f35-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
