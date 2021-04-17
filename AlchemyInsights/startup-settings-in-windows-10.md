---
title: Startinställningar i Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828170"
---
# <a name="startup-settings-in-windows-10"></a>Startinställningar i Windows 10

**Ändra vilka appar som körs automatiskt vid start**

1. Gå till [Inställningar > Program > Start](ms-settings:startupapps?activationSource=GetHelp).

2. Kontrollera att alla appar som du vill köra vid start **är** på .

**Lägga till ett program som ska köras automatiskt vid start**

1. Klicka eller tryck **på Start** och leta reda på programmet du vill köra vid start.

2. Högerklicka på programmet, klicka på **Mer och** klicka sedan på **Öppna filplats**. Då öppnas den plats där genvägen till programmet sparas. Om det inte finns något alternativ för Öppna filplats betyder det att programmet inte kan köras vid start.

3. Med filplatsen öppen trycker du på **Windows-tangenten + R,** skriver **shell:startup** och klickar sedan på **OK.** Då öppnas mappen Autostart.

4. Kopiera och klistra in genvägen till programmet från filens plats i startmappen.

**Avancerade startalternativ (inklusive felsäkert läge, UEFI-inställningar och start från en annan enhet)**

1. Spara ditt arbete och stäng alla öppna dokument eftersom de här stegen startar om datorn.

2. Gå till [Inställningar > Uppdatering & Säkerhetsinställningar > Återställning](ms-settings:recovery?activationSource=GetHelp).

3. Klicka **på Starta om** nu under Avancerad **start.** 

4. När datorn startats om till skärmen Välj ett alternativ:

    - Om du vill starta från en enhet som en USB-enhet klickar du **på Använd en enhet**.

    - Om du vill ange UEFI-inställningarna (kallas ibland FÖR TIDSKONFIGURATION) klickar du **> Avancerade alternativ > inbyggd UEFI-inställning.** 

    - Om du vill öppna felsäkert läge eller ändra avancerade startinställningar klickar du > På avancerade **> inställningar** och sedan på Starta **om**. Du kan bli ombedd att ange din [BitLocker-återställningsnyckel](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). När datorn har startats om igen klickar du på den startinställning du vill använda.