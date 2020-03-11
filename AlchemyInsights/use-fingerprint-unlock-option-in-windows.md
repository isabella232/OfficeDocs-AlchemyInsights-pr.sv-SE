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
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Använda alternativet för upplåsning av fingeravtryck i Windows 10

**Aktivera Windows Hello Fingerprint**

Om du vill låsa upp Windows 10 med ditt fingeravtryck måste du konfigurera Windows Hello Fingerprint genom att lägga till (låta Windows lära sig känna igen) minst ett finger. 

1. Gå till **Inställningar > konton > inloggningsalternativ** (eller klicka [här).](ms-settings:signinoptions?activationSource=GetHelp) Tillgängliga inloggningsalternativ visas. Till exempel:

    ![Inloggningsalternativ.](media/sign-in-options.png)

2. Klicka eller tryck på **Windows Hello Fingerprint**och sedan på **Konfigurera**. Klicka på **Kom igång**i installationsfönstret för Windows Hello. Fingeravtryckssensorn aktiveras och du blir ombedd att placera fingret på sensorn:

   ![Fingeravtryckssensor.](media/fingerprint-sensor.png)

3. Följ instruktionerna, som kommer att be dig att upprepade gånger skanna fingret. När detta är klart har du möjlighet att lägga till andra fingrar som du kanske vill använda för inloggning. Nästa gång du loggar in på Windows 10 har du möjlighet att använda ditt fingeravtryck för att göra det.

**Windows Hello Fingerprint är inte tillgängligt som inloggningsalternativ**

Om Windows Hello Fingerprint inte visas som ett alternativ i **inloggningsalternativ**betyder det att Windows inte känner till någon fingeravtrycksläsare/skanner som är ansluten till datorn eller att en systemprincip förhindrar dess användning (om till exempel datorn hanteras av din arbetsplats). Så här felsöker du: 

1. Välj **Start-knappen** i Aktivitetsfältet och sök efter **Enhetshanteraren**.

2. Öppna **Enhetshanteraren**genom att klicka eller trycka.

3. Expandera Biometriska enheter i Enhetshanteraren genom att klicka på dess sparrar.

   ![Biometriska enheter.](media/biometric-devices.png)

4. Fingeravtrycksskannern ska listas som en biometrisk enhet, till exempel Synaptics WBDI-skannern:

   ![Biometriska enheter.](media/biometric-devices-expanded.png)

5. Om fingeravtrycksskannern inte visas och skannern är integrerad i datorn går du till datortillverkarens webbplats. I avsnittet teknisk support för din datormodell söker du efter en Windows 10-drivrutin efter en skanner som du kan installera.

6. Om skannern är skild från datorn (ansluten via USB) går du till skannertillverkarens webbplats för att hitta och installera Windows 10-drivrutinsprogram för den skannermodell du har.
