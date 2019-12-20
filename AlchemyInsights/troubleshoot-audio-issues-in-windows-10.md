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
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796411"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a>Felsöka ljudproblem i Windows 10

**Kör felsökaren för ljud**

Ljudfelsökaren kanske kan åtgärda ljudproblemen automatiskt: 

1. Välj **Start**, Skriv **Felsök**och välj sedan **Felsök** i listan med resultat. 
2. Välj **spela upp ljud** > **Kör felsökaren**.

**Kontrollera kablar, volym, högtalare och hörlurar**

- Kontrollera högtalar-och hörlurs anslutningarna för lösa kablar och kontrollera att de är anslutna till rätt uttag.
- Kontrollera ström-och volymnivåerna och försök att vrida alla volymkontrollerna uppåt.
- Vissa högtalare och appar har egna volymkontroller, och du kan behöva kontrollera dem alla för att se till att de är på rätt nivå.
- Prova att ansluta med en annan USB-port.
- **Anmärkning:** Kom ihåg att högtalarna kanske inte fungerar när hörlurarna är anslutna.

**Kontrollera Enhetshanteraren**

Så här kontrollerar du att drivrutinerna är uppdaterade:

- Välj **Start**, Skriv **Enhetshanteraren**och välj sedan **Enhetshanteraren** i listan med resultat.

2. Under **ljud-, video-och spelenheter**väljer du ljudkortet, öppnar det, väljer fliken **drivrutin** och väljer **Uppdatera drivrutin**. 

**Anmärkning:** Om Windows inte hittar en ny drivrutin letar du efter en på enhetstillverkarens webbplats och följer deras instruktioner.

**Installera om drivrutinen**

Om du inte kan uppdatera via Enhetshanteraren eller hitta en ny drivrutin på tillverkarens webbplats provar du dessa steg: 

1. Högerklicka på (eller håll ned) ljuddrivrutinen i Enhetshanteraren och välj **Avinstallera**. Starta om enheten så försöker Windows att installera om drivrutinen.

2. Om ominstallation av drivrutinen inte fungerar provar du att använda den generiska ljuddrivrutinen som medföljer Windows. I Enhetshanteraren, högerklicka (eller tryck och håll) ljuddrivrutinen > **Uppdatera drivrutinsprogramvara** > **Bläddra min dator för drivrutinsprogramvara** > **Låt mig välja från en lista över drivrutiner på min dator**, Välj **High Definition ljudenhet**, Välj **Nästa**, och följ instruktionerna för att installera den.

**Ställa in standardenhet**

Om du ansluter till en ljudenhet med USB eller HDMI kan du behöva ställa in den enheten som standard: 

1. Välj **Start**, Skriv **ljud**och välj sedan **ljud** eller **ändra systemljud** i listan med resultat.

2. Välj en enhet på fliken **uppspelning** , Välj **standard**och välj sedan **OK**.

