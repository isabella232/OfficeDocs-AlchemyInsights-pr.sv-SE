---
title: Felsöka ljudproblem i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265034"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Felsökning av ljudproblem i Windows 10

**Kör felsökaren för ljud**

1.  Öppna [felsöksinställningarna](ms-settings:troubleshoot).

2.  Välj **Spela upp ljud** > **Kör felsökaren**.

**Ange standardenheten**

Om du ansluter till en ljudenhet med USB eller HDMI kan du behöva ställa in enheten som standard:

1. Öppna **Startljud** > **** och välj sedan **Ljud-** eller **ändringssystemljud** från resultatlistan.

2.  Välj en enhet på fliken Uppspelning **** på fliken **Uppspelning** och välj sedan **OK**.

**Kontrollera kablar, volym, högtalare och hörlurar**

1. Kontrollera att högtalaren och hörlursanslutningarna är anslutna till rätt uttag.

2. Kontrollera dina effekt- och volymnivåer och försök att vrida upp alla volymkontroller.

3. Vissa högtalare och appar har sina egna volymkontroller. Du kanske måste kontrollera dem alla för att se till att de är på rätt nivåer.

4. Prova att ansluta med en annan USB-port.

**Kom ihåg**att högtalarna kanske inte fungerar när hörlurar är anslutna.

**Kontrollera Enhetshanteraren**

Så här kontrollerar du att drivrutinerna är uppdaterade:

1. Välj **Start,** skriv **Enhetshanteraren**och välj sedan **Enhetshanteraren** i resultatlistan.

2. Under **Ljud-, video- och spelkontroller**väljer du ljudkortet, öppnar det, väljer fliken **Drivrutin** och väljer **Uppdatera drivrutinen**.

**Om**Windows inte hittar en ny drivrutin letar du efter en på enhetstillverkarens webbplats och följer deras instruktioner.

**Installera om drivrutinen**

Om du inte kan uppdatera via Enhetshanteraren eller hitta en ny drivrutin på tillverkarens webbplats kan du prova följande:

1. Högerklicka (eller håll ned) ljuddrivrutinen i Enhetshanteraren och välj **Avinstallera**. Starta om enheten och Windows försöker installera om drivrutinen.

2. Om omduinstallerar drivrutinen inte fungerar kan du prova att använda den generiska ljuddrivrutinen som medföljer Windows. Högerklicka (eller håll ned) ljuddrivrutinen > **Uppdatera drivrutinsprogramvaran** > **Bläddra i datorn för drivrutinsprogram** > Låt mig välja från en lista över drivrutiner på**datorn,** välj **Hd-ljudenhet**, välj **Nästa**och följ instruktionerna för att installera den.
