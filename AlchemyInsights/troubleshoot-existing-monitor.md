---
title: Felsöka befintlig bildskärm
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690729"
---
# <a name="troubleshoot-an-existing-monitor"></a>Felsöka en befintlig bildskärm

Prova de här lösningarna för att felsöka en bildskärm. 

**Uppdatera bildskärmens skärm:**

Tryck på följande tangenter samtidigt: Windows-tangenten + Ctrl + Skift + B. Då uppdateras kommunikationen med grafik driv rutinen. Dina skärmar blinkar tillfälligt och kommer tillbaka efter några sekunder.

**Felsöka skärm maskin vara:**

1. Koppla bort kabeln som ansluter datorn till din bildskärm och koppla in den igen.
2. Koppla bort alla icke-väsentliga enheter från datorn (till exempel adaptrar eller dock).

**Om du nyligen har installerat en uppdatering på datorn kan du återställa bildskärmens driv rutinen:**

1. Välj **Start**, Skriv **enhets hanteraren**och välj **enhets hanteraren** från resultaten.
2. Expandera avsnittet **bildskärms kort** , högerklicka på bildskärms kortet, Ands Välj **Egenskaper**.
3. Gå till fliken **driv rutin** och välj **Återställ driv rutin**. <br>
OBS! om det inte är tillgängligt eller är nedtonat väljer du **Nej** från alternativen nedan för att gå till nästa steg.
4. Du kan behöva starta om datorn innan ändringarna börjar gälla.

**Avinstallera och installera om bildskärms driv rutinen:**

1. Välj **Start**, Skriv **enhets hanteraren**och välj **enhets hanteraren** från resultaten.
2. Expandera avsnittet **bildskärms kort** , högerklicka på bildskärms kortet, Ands Välj **Avinstallera enhet**. 
3. Markera rutan bredvid **ta bort driv rutinen för den här enheten** och välj **Avinstallera**.<br>
Obs! Du kan uppmanas att starta om datorn i den här fasen. Skriv ned de återstående anvisningarna innan du startar om.
4. Öppna enhets hanteraren igen.
5. Expandera avsnittet **bildskärms kort** , högerklicka på bildskärms kortet och välj **Uppdatera driv rutin**.
6. Välj **Sök automatiskt för uppdatera driv rutiner** och följ installations anvisningarna.