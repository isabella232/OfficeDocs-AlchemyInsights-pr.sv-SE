---
title: Använda alternativet för upplåsning av fingeravtryck i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588333"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="382a4-102">Använda alternativet för upplåsning av fingeravtryck i Windows 10</span><span class="sxs-lookup"><span data-stu-id="382a4-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="382a4-103">**Aktivera Windows Hello Fingerprint**</span><span class="sxs-lookup"><span data-stu-id="382a4-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="382a4-104">Om du vill låsa upp Windows 10 med ditt fingeravtryck måste du konfigurera Windows Hello Fingerprint genom att lägga till (låta Windows lära sig känna igen) minst ett finger.</span><span class="sxs-lookup"><span data-stu-id="382a4-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="382a4-105">Gå till **Inställningar > konton > inloggningsalternativ** (eller klicka [här).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="382a4-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="382a4-106">Tillgängliga inloggningsalternativ visas.</span><span class="sxs-lookup"><span data-stu-id="382a4-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="382a4-107">Till exempel:</span><span class="sxs-lookup"><span data-stu-id="382a4-107">For example:</span></span>

    ![Inloggningsalternativ.](media/sign-in-options.png)

2. <span data-ttu-id="382a4-109">Klicka eller tryck på **Windows Hello Fingerprint**och sedan på **Konfigurera**.</span><span class="sxs-lookup"><span data-stu-id="382a4-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="382a4-110">Klicka på **Kom igång**i installationsfönstret för Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="382a4-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="382a4-111">Fingeravtryckssensorn aktiveras och du blir ombedd att placera fingret på sensorn:</span><span class="sxs-lookup"><span data-stu-id="382a4-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Fingeravtryckssensor.](media/fingerprint-sensor.png)

3. <span data-ttu-id="382a4-113">Följ instruktionerna, som kommer att be dig att upprepade gånger skanna fingret.</span><span class="sxs-lookup"><span data-stu-id="382a4-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="382a4-114">När detta är klart har du möjlighet att lägga till andra fingrar som du kanske vill använda för inloggning.</span><span class="sxs-lookup"><span data-stu-id="382a4-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="382a4-115">Nästa gång du loggar in på Windows 10 har du möjlighet att använda ditt fingeravtryck för att göra det.</span><span class="sxs-lookup"><span data-stu-id="382a4-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="382a4-116">**Windows Hello Fingerprint är inte tillgängligt som inloggningsalternativ**</span><span class="sxs-lookup"><span data-stu-id="382a4-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="382a4-117">Om Windows Hello Fingerprint inte visas som ett alternativ i **inloggningsalternativ**betyder det att Windows inte känner till någon fingeravtrycksläsare/skanner som är ansluten till datorn eller att en systemprincip förhindrar dess användning (om till exempel datorn hanteras av din arbetsplats).</span><span class="sxs-lookup"><span data-stu-id="382a4-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="382a4-118">Så här felsöker du:</span><span class="sxs-lookup"><span data-stu-id="382a4-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="382a4-119">Välj **Start-knappen** i Aktivitetsfältet och sök efter **Enhetshanteraren**.</span><span class="sxs-lookup"><span data-stu-id="382a4-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="382a4-120">Öppna **Enhetshanteraren**genom att klicka eller trycka.</span><span class="sxs-lookup"><span data-stu-id="382a4-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="382a4-121">Expandera Biometriska enheter i Enhetshanteraren genom att klicka på dess sparrar.</span><span class="sxs-lookup"><span data-stu-id="382a4-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometriska enheter.](media/biometric-devices.png)

4. <span data-ttu-id="382a4-123">Fingeravtrycksskannern ska listas som en biometrisk enhet, till exempel Synaptics WBDI-skannern:</span><span class="sxs-lookup"><span data-stu-id="382a4-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometriska enheter.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="382a4-125">Om fingeravtrycksskannern inte visas och skannern är integrerad i datorn går du till datortillverkarens webbplats.</span><span class="sxs-lookup"><span data-stu-id="382a4-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="382a4-126">I avsnittet teknisk support för din datormodell söker du efter en Windows 10-drivrutin efter en skanner som du kan installera.</span><span class="sxs-lookup"><span data-stu-id="382a4-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="382a4-127">Om skannern är skild från datorn (ansluten via USB) går du till skannertillverkarens webbplats för att hitta och installera Windows 10-drivrutinsprogram för den skannermodell du har.</span><span class="sxs-lookup"><span data-stu-id="382a4-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
