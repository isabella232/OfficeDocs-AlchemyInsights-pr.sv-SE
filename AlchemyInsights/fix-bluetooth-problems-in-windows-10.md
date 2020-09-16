---
title: Åtgärda problem med Bluetooth i Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730177"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Åtgärda problem med Bluetooth i Windows 10

Om Bluetooth-ikonen saknas eller om det inte går att aktivera eller inaktivera Bluetooth kan du köra fel sökaren för Bluetooth. [Öppna fel söknings inställningar](ms-settings:troubleshoot), klicka på **Bluetooth** under **hitta och åtgärda andra problem**klickar **du på kör fel sökaren**.

Om du inte ser Bluetooth-ikonen men Bluetooth visas i enhets hanteraren:

1. Klicka på **Bluetooth**i enhets hanteraren. Tryck och håll ned (eller högerklicka på) namnet på Bluetooth-kortet och klicka på **Avinstallera enhet**.

2. Stäng av Windows-enheten, vänta några sekunder och slå sedan på den igen. Windows försöker installera om driv rutinen.

Om du nyligen har installerat uppdateringar för Windows 10 eller uppgraderat till Windows 10 kan det vara bra att söka efter driv rutins uppdateringar:

1. Klicka på **Bluetooth**i enhets hanteraren och klicka sedan på namnet på Bluetooth-kortet (som kan innehålla ordet "Radio").

2. Håll ned (eller högerklicka) på Bluetooth-kortet och klicka sedan på Uppdatera Sök efter **driv rutin**  >  **automatiskt för uppdaterade driv rutiner**. Följ stegen och klicka sedan på **Stäng**.

      - Om Windows inte hittar en ny Bluetooth-drivrutin kan du besöka PC-tillverkarens webbplats och ladda ner den senaste Bluetooth-drivrutinen därifrån.

    - När du har laddat ner det klickar du på **Uppdatera driv rutin**  >  **Bläddra på datorn efter driv rutiner**  >  **Bläddra** efter den plats där drivrutinsfilerna lagras > **OK**  >  **Nästa**och följer anvisningarna för att installera.

3. När du har installerat den uppdaterade driv rutinen startar du om datorn och kontrollerar sedan om det löser anslutnings problemet.

Mer information om hur du felsöker Bluetooth-problem finns i artikeln om att [åtgärda Bluetooth-problem i Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).
