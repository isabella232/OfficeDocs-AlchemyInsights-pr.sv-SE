---
title: 'Fel: reglerna på den här datorn stämmer inte överens'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690981"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fel: reglerna på den här datorn stämmer inte överens

Om du vill se uppdaterad status för det här kända problemet läser [du reglerna på den här datorn stämmer inte överens med reglerna för Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook-teamet har implementerat en korrigering i version 12928,10000. Korrigeringen är redan i Insider – snabbt och kommer att gå till månads kanal i 2020 i sent juni. När du har den fasta versionen kan du få meddelandet "vilka regler vill du behålla" en sista gång. Välj server när du uppmanas till det och gå tillbaka till Outlook och återaktivera eventuella regler som inaktiverats.

När korrigeringen är tillgänglig kan du använda följande lösning:

**Lösning**: problemet har uppstått i de senaste rapporterna för dem som bara har skapat klient regler i Outlook-skrivbordet. Om du fortsätter med problemet kan du överväga att ta bort reglerna och sedan skapa och redigera regler endast i OWA (Outlook Web App) tills problemet är löst.

Om du inte kan ta bort reglerna manuellt kan du köra ett Outlook-kommando när du startar Outlook genom att köra Outlook.exe/Cleanrules. Detta tar bort både klient-och Server reglerna. Alla regler för alla konton i Outlook-profilen tas bort. Det här kommandot dokumenteras också i artikeln kommando rads växlar.

