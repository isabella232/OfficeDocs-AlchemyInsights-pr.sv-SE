---
title: Åtgärda Bluetooth problem i Windows 10
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
ms.openlocfilehash: 784f8c4d58bb8965cec2ce0a3722d0f16e36b16f914b4a154d6f6da58af9dc28
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53913913"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Åtgärda Bluetooth problem i Windows 10

Om Bluetooth ikon saknas eller om Bluetooth inte kan aktiveras eller inaktiveras kan det vara bra att köra felsökaren Bluetooth felsökaren. [Öppna felsökningsinställningarna,](ms-settings:troubleshoot)klicka **Bluetooth** under **Hitta och åtgärda andra problem** och klicka på Kör **felsökaren.**

Om du inte ser ikonen Bluetooth, men Bluetooth visas i Enhetshanteraren:

1. I Enhetshanteraren klickar du **på Bluetooth**. Håll ned (eller högerklicka på) namnet på Bluetooth adaptern och klicka på **Avinstallera enhet.**

2. Avsluta enheten Windows, vänta några sekunder och aktivera den sedan igen. Windows försöker installera om drivrutinen.

Om du nyligen installerat Windows 10 uppdateringar eller uppgraderat till Windows 10 kan du söka efter drivrutinsuppdateringar:

1. I Enhetshanteraren klickar du **Bluetooth** och sedan på Bluetooth kortnamnet (vilket kan inkludera ordet "radio").

2. Håll ned (eller högerklicka på) Bluetooth kort och klicka sedan på **Sök efter** uppdaterade drivrutiner  >  **automatiskt.** Följ anvisningarna och klicka sedan på **Stäng.**

      - Om Windows kan hitta en ny Bluetooth drivrutin går du till datortillverkarens webbplats och laddar ned den senaste Bluetooth drivrutinen därifrån.

    - När du har laddat ned den klickar du på Uppdatera drivrutin Bläddra i datorn efter drivrutinsprogramvara Bläddra efter den plats där drivrutinsfilerna lagras > OK Nästa och följ anvisningarna  >    >   för   >  att installera.

3. När du har installerat den uppdaterade drivrutinen startar du om datorn och kontrollerar om det löser problemet.

Mer information om hur du felsöker Bluetooth finns i den fullständiga artikeln, [Åtgärda problem Bluetooth i Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)
