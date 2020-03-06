---
title: Startinställningar i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409227"
---
# <a name="startup-settings-in-windows-10"></a>Startinställningar i Windows 10

**Ändra vilka appar som körs automatiskt vid start**

1. Gå till [Inställningar > Apps > Start](ms-settings:startupapps?activationSource=GetHelp).

2. Kontrollera att alla appar som du vill köra vid start är **påslagna**.

**Lägga till en app som ska köras automatiskt vid start**

1. Klicka eller tryck på **Start** och leta reda på appen som du vill köra vid start.

2. Högerklicka på appen, klicka på **Mer**och klicka sedan på **Öppna filplats**. På så sätt öppnas platsen där genvägen till appen sparas. Om det inte finns något alternativ för Öppna filplats betyder det att appen inte kan köras vid start.

3. När filplatsen är öppen trycker du på **Windows-tangenten + R,** skriver **shell:startup**och klickar sedan på **OK**. Då öppnas startmappen.

4. Kopiera och klistra in genvägen till appen från filplatsen till startmappen.

**Avancerade startalternativ (inklusive felsäkert läge, UEFI-inställningar och uppstart från en annan enhet)**

1. Spara ditt arbete och stäng alla öppna dokument, eftersom dessa steg startar om datorn.

2. Gå till [Inställningar > Uppdatera & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. Klicka på **Starta om nu under**Avancerad **start**. 

4. När datorn har startats om till skärmen Välj ett alternativ:

    - Om du vill starta från en enhet som en USB-enhet klickar du på **Använd en enhet**.

    - Om du vill ange UEFI-inställningarna (kallas ibland BIOS-inställningar) klickar du **på Felsöka > avancerade alternativ > UEFI-inställningar för inbyggd programvara**. 

    - Om du vill ange felsäkert läge eller ändra avancerade startinställningar klickar du på **Felsöka > Avancerade alternativ > startinställningar**och sedan på **Starta om**. Du kan bli ombedd att ange [din BitLocker-återställningsnyckel](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). När datorn har startats om igen klickar du på den startinställning som du vill använda.