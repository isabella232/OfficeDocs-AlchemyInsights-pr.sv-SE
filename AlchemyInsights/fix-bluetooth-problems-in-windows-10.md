---
title: Åtgärda Bluetooth-problem i Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812950"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Åtgärda Bluetooth-problem i Windows 10

Om Bluetooth-ikonen saknas eller om Bluetooth inte kan aktiveras eller inaktiveras kan du köra Bluetooth-felsökaren. [Öppna felsökningsinställningarna](ms-settings:troubleshoot), klicka på **Bluetooth** under **Hitta och åtgärda andra problem** och klicka på Kör **felsökaren.**

Om Bluetooth-ikonen inte visas, men Bluetooth visas i Enhetshanteraren:

1. Klicka på Bluetooth i **Enhetshanteraren.** Håll ned (eller högerklicka på) Bluetooth-adapterns namn och klicka på **Avinstallera enhet**.

2. Stäng av Windows-enheten, vänta några sekunder och aktivera den sedan igen. Windows försöker installera om drivrutinen.

Om du nyligen har installerat Windows 10-uppdateringar eller uppgraderat till Windows 10 kanske du vill söka efter drivrutinsuppdateringar:

1. I Enhetshanteraren klickar du **på Bluetooth** och sedan på namnet på Bluetooth-adaptern (vilket kan inkludera ordet "radio").

2. Håll ned (eller högerklicka på) Bluetooth-adaptern och klicka sedan på **Uppdatera**  >  **drivrutinssökning automatiskt för uppdaterad drivrutinsprogramvara.** Följ anvisningarna och klicka sedan på **Stäng.**

      - Om Windows inte kan hitta en ny Bluetooth-drivrutin går du till datortillverkarens webbplats och laddar ned den senaste Bluetooth-drivrutinen därifrån.

    - När du har laddat ned den klickar du på Uppdatera drivrutin Bläddra i datorn efter drivrutinsprogramvara Bläddra efter den plats där drivrutinsfilerna lagras > OK Nästa och följ anvisningarna  >    >   för   >  att installera.

3. När du har installerat den uppdaterade drivrutinen startar du om datorn och kontrollerar om det löser problemet.

Mer information om hur du felsöker Bluetooth-problem finns i den fullständiga artikeln Åtgärda [Bluetooth-problem i Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)
