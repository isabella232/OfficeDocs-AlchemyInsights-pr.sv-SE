---
title: Felsöka ljudproblem i Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 81a7f77bd6565c52ec9d752934a872e59cc11e89b90a646d17c3549d72e8a69f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039444"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Felsöka ljudproblem i Windows 10

**Köra felsökaren för ljud**

1.  Öppna [felsökningsinställningarna.](ms-settings:troubleshoot)

2.  Välj **Ljuduppspelning**  >  **Kör felsökaren**.

**Ange standardenhet**

Om du ansluter till en ljudenhet med USB eller HDMI kan du behöva ange den enheten som standardenhet:

1. Öppna **Starta**  >  **ljud** och välj sedan **Ljud eller** Ändra **systemljud** i listan med resultat.

2.  Välj **en enhet** på fliken Uppspelning, välj **Ange standard** och välj sedan **OK.**

**Kontrollera kablar, volym, högtalare och hörlurar**

1. Kontrollera att alla kablar är korrekt anslutna i högtalarna och hörlurarna och att de är anslutna till rätt uttag.

2. Kontrollera ström och volym, och prova att vrida upp alla volymkontroller.

3. Vissa högtalare och appar har egna volymkontroller. du kanske måste kontrollera alla för att säkerställa att de är på rätt nivåer.

4. Prova att ansluta via en annan USB-port.

**Obs!** Kom ihåg att högtalarna kanske inte fungerar när hörlurar är inkopplade.

**Kontrollera Enhetshanteraren**

Så här kontrollerar du att drivrutinerna är uppdaterade:

1. Välj **Start**, **skriv Enhetshanteraren** och välj **sedan Enhetshanteraren** i listan med resultat.

2. Under **Ljud-, video- och spelenheter** väljer du ditt ljudkort, öppnar det, väljer fliken **Drivrutin** och väljer Uppdatera **drivrutin.**

**Obs!** Windows du inte hittar en ny drivrutin letar du upp en på enhetstillverkarens webbplats och följer deras instruktioner.

**Installera om drivrutinen**

Om du inte kan uppdatera via Enhetshanteraren eller hitta en ny drivrutin på tillverkarens webbplats kan du prova följande:

1. I Enhetshanteraren högerklickar du på (eller håller ned) ljuddrivrutinen och väljer **Avinstallera.** Starta om enheten så Windows att försöka installera om drivrutinen.

2. Om det inte fungerar att installera om drivrutinen kan du prova att använda den allmänna ljuddrivrutinen som medföljer Windows. I Enhetshanteraren högerklickar du på (eller håller ned) din ljuddrivrutin > Uppdatera drivrutinsprogramvara Bläddra i datorn efter drivrutinsprogramvara Låt mig välja från en lista med drivrutiner på datorn , välj High Definition Audio Device , välj Nästa och följ anvisningarna för att installera  >    >  den.  
