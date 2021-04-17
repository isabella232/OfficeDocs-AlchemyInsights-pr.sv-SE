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
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824597"
---
# <a name="troubleshoot-an-existing-monitor"></a>Felsöka en befintlig bildskärm

Prova de här lösningarna för att felsöka en bildskärm. 

**Uppdatera bildskärmen:**

Tryck på följande tangenter samtidigt: Windows-tangenten + Ctrl + Skift + B. Det här uppdaterar kommunikationen med grafikdrivrutinen. Bildskärmarna blinkar tillfälligt och kommer tillbaka efter några sekunder.

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