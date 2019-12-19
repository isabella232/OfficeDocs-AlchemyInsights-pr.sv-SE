---
title: Felsöka befintlig bildskärm
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738586"
---
# <a name="troubleshoot-an-existing-monitor"></a>Felsöka en befintlig bildskärm

Prova dessa lösningar för att felsöka en bildskärm. 

**Uppdatera bildskärmens display:**

Tryck på följande tangenter samtidigt: Windows-tangenten + Ctrl + Skift + B. Detta kommer att uppdatera kommunikationen med din grafikdrivrutin. Dina bildskärmar kommer att blinka tillfälligt och komma tillbaka efter några sekunder.

**Felsöka bildskärms maskinvara:**

1. Koppla bort kabeln som ansluter datorn till bildskärmen och Anslut den igen.
2. Koppla bort alla icke-nödvändiga enheter från datorn (till exempel adaptrar eller dockor).

**Om du nyligen har installerat en uppdatering på datorn kan du återställa bildskärmsdrivrutinen:**

1. Välj **Start**, Skriv **Enhetshanteraren**och välj **Enhetshanteraren** i resultatet.
2. Expandera avsnittet **bildskärmskort** , högerklicka på bildskärmskortet, Ands Välj **Egenskaper**.
3. Navigera till fliken **drivrutin** och välj **Återställ tillbaka drivrutin**. <br>
Om detta inte är tillgängligt eller är nedtonat väljer du **Nej** i alternativen nedan för att gå vidare till nästa steg.
4. Du kan behöva starta om datorn innan ändringarna träder i kraft.

**Avinstallera och installera om bildskärmsdrivrutinen:**

1. Välj **Start**, Skriv **Enhetshanteraren**och välj **Enhetshanteraren** i resultatet.
2. Expandera avsnittet **bildskärmskort** , högerklicka på bildskärmskortet, Ands Välj **Avinstallera enhet**. 
3. Markera rutan bredvid **ta bort drivrutinsprogramvaran för den här enheten** och välj **Avinstallera**.<br>
Obs: du kan bli ombedd att starta om datorn i detta skede. Se till att anteckna de återstående instruktionerna innan du startar om.
4. Öppna Enhetshanteraren igen.
5. Expandera avsnittet **bildskärmskort** , högerklicka på bildskärmskortet och välj **Uppdatera drivrutin**.
6. Välj **Sök automatiskt efter uppdatera drivrutinsprogramvara** och följ installationsanvisningarna.