---
title: Felsöka befintlig bildskärm
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
- "3454"
- "9001450"
ms.openlocfilehash: 2ecfb4e90f2d58654ec43a35e901ea4421e0e94fa95995ef890abc8af2d99ec7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981095"
---
# <a name="troubleshoot-an-existing-monitor"></a>Felsöka en befintlig bildskärm

Prova de här lösningarna för att felsöka en bildskärm. 

**Uppdatera bildskärmen:**

Tryck på följande tangenter samtidigt: Windows + Ctrl + Skift + B. Det här uppdaterar kommunikationen med grafikdrivrutinen. Bildskärmarna blinkar tillfälligt och kommer tillbaka efter några sekunder.

**Felsöka maskinvara för bildskärmen:**

1. Koppla ur kabeln som ansluter datorn till bildskärmen och anslut den igen.
2. Koppla bort alla enheter som inte är nödvändiga från datorn (till exempel adaptrar eller dockor).

**Om du nyligen har installerat en uppdatering på datorn kan du återställa bildskärmsdrivrutinen:**

1. Välj **Start**, **skriv enhetshanteraren** och **välj Enhetshanteraren** i resultatet.
2. Expandera avsnittet **Bildskärmskort,** högerklicka på bildskärmskortet och välj **Egenskaper**.
3. Gå till fliken **Drivrutin** och välj **Återställ drivrutin.** <br>
Obs! Om det här inte är tillgängligt eller är nedtonat väljer du **Nej** i alternativen nedan för att gå vidare till nästa steg.
4. Du kan behöva starta om datorn innan ändringarna börjar gälla.

**Avinstallera och installera om din bildskärmsdrivrutin:**

1. Välj **Start**, **skriv enhetshanteraren** och **välj Enhetshanteraren** i resultatet.
2. Expandera avsnittet **Bildskärmskort,** högerklicka på bildskärmskortet och välj **Avinstallera enhet**. 
3. Markera rutan bredvid Ta **bort drivrutinsprogramvaran för den här enheten** och välj **Avinstallera**.<br>
Obs! Du kan bli ombedd att starta om datorn i det här läget. Skriv ned resten av instruktionerna innan du startar om.
4. Öppna Enhetshanteraren igen.
5. Expandera avsnittet **Bildskärmskort,** högerklicka på bildskärmskortet och välj **Uppdatera drivrutin.**
6. Välj **Sök automatiskt efter programvara för uppdatering av drivrutinen** och följ installationsanvisningarna.