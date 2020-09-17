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
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Använd alternativet för att låsa upp finger i Windows 10

**Aktivera finger avtryck för Windows Hello**

För att låsa upp Windows 10 med ditt finger avtryck måste du konfigurera Windows Hello-finger avtryck genom att lägga till (och låta Windows lära sig känna igen) minst ett finger. 

1. Gå till **inställningar > konton > inloggnings alternativ** (eller klicka [här](ms-settings:signinoptions?activationSource=GetHelp)). Tillgängliga inloggnings alternativ visas. Ett exempel:

    ![Inloggnings alternativ.](media/sign-in-options.png)

2. Klicka eller tryck på **Windows Hello-finger avtryck**och sedan på **Konfigurera**. I fönstret Windows Hello-inställningar klickar du på **komma igång**. Finger avtrycks sensorn aktive ras och du uppmanas att placera fingret på sensorn:

   ![Finger avtryck.](media/fingerprint-sensor.png)

3. Följ instruktionerna som ber dig att upprepade gånger kontrol lera ditt finger. När det är klart kan du välja att lägga till andra fingrar som du kan använda för inloggning. Nästa gång du loggar in i Windows 10 kan du välja att använda ditt finger avtryck för att göra det.

**Windows Hello-finger avtryck är inte tillgängligt som inloggnings alternativ**

Om Windows Hello-finger avtryck inte visas som ett alternativ i **inloggnings alternativ**innebär det att Windows inte känner till vilken finger avtrycks läsare/skanner som är ansluten till datorn eller att en system princip hindrar dess användning (om till exempel din dator hanteras av din arbets plats). Så här felsöker du: 

1. Välj **Start** -knappen i aktivitets fältet och Sök efter **enhets hanteraren**.

2. Klicka eller tryck för att öppna **enhets hanteraren**.

3. I enhets hanteraren expanderar du bio metriska enheter genom att klicka på dess gränssnitt.

   ![Bio metriska enheter.](media/biometric-devices.png)

4. Din finger avtrycks läsare ska visas som en bio Metrisk enhet, till exempel Synaptics WBDI-skanner:

   ![Bio metriska enheter.](media/biometric-devices-expanded.png)

5. Om din finger avtrycks läsare inte visas och skannern är inbyggd i datorn går du till tillverkarens webbplats. I avsnittet teknisk support för dator modellen söker du efter en Windows 10-drivrutin för en skanner som du kan installera.

6. Om skannern är avgränsad från datorn (ansluten via USB) går du till skanner tillverkarens webbplats för att hitta och installera Windows 10-enhets driv rutiner för den skanner modell du har.
