---
title: Om Exchange Server säkerhetsuppdateringar
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482986"
---
# <a name="about-exchange-server-security-updates"></a>Om Exchange Server säkerhetsuppdateringar

Microsoft har släppt en serie kritiska säkerhetsuppdateringar för Exchange Server lokalt. De aktuella serverversionerna är uppdateringsnivåer för Exchange Server 2010, 2013, 2016 och 2019. Exchange Online påverkas INTE, men om du har några lokala Exchange-servrar på grund av hybridkonfigurationen är de potentiellt sårbara.

Om du vill uppdatera dina lokala servrar måste du köra minst följande versioner av Exchange:

- Exchange 2010 Service Pack 3
- Exchange Server 2013 CU 23
- Exchange Server 2016 CU 19 eller CU 18
- Exchange Server 2019 CU 8 eller CU 7

Se följande meddelande om placeringen av korrigeringar: [släpptes: mars 2021 Exchange Server säkerhetsuppdateringar](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)

**Viktiga kommentarer:**

Installation av uppdateringar fungerar inte om dina lokala servrar inte kör nödvändiga Exchange-versioner, enligt ovanstående lista.

Om du installerar uppdateringar manuellt läser du avsnittet "Kända problem" i KB-uppdateringsartiklarna för viktig information. Säkerhetsuppdateringar MÅSTE köras från cmd/PowerShell-uppmaningen för förhöjda cmd!
