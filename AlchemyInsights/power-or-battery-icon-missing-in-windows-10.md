---
title: Ikonen för ström eller batteriet saknas i Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 82d41844de1eafdf7e0cc38f91416f3b71868e3d5d1b3eb8be0f10abd701ddc8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973365"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Ikonen för ström eller batteriet saknas i Windows 10

Om din Windows 10-enhet har ett batteri (t.ex. en bärbar dator, surfplatta eller en dator ansluten via USB till en UPS) visas vanligtvis en ikon för ström eller batteri i aktivitetsfältet nära klockan, till exempel:

![Batteriets ikon](media/battery-icon.png)

Om den här ikonen inte visas kan den vara dold:

1. Gå till **[Inställningar > Anpassning > Aktivitetsfältet](ms-settings:taskbar?activationSource=GetHelp)**.

2. I meddelandefältet klickar du på **Välj vilka ikoner som ska visas i Aktivitetsfältet**.

3. Leta sedan efter objektet för **Ström** i listan och ändra inställningen till **På**.

    ![Visa ikon för Ström i Aktivitetsfältet](media/power-icon-on.png)

**Felsökning**

Om du följde anvisningarna ovan och knappen för **Ström** är nedtonad eller inte visas går du till sökrutan i Aktivitetsfältet och skriver in **Enhetshanteraren**, välj sedan **Enhetshanteraren** i resultatlistan. Via **Batterier** högerklickar du på enhetens batteri, klicka på **Inaktivera** och sedan på **Ja**. Vänta några sekunder och högerklicka sedan på batteriet och klicka på **Aktivera**. Starta sedan om enheten.

Om du följde anvisningarna ovan men ikonen för batteriet visas inte i aktivitetsfältet går du till sökrutan i Aktivitetsfältet och skriver in **Aktivitetshanteraren**, klicka sedan på **Aktivitetshanteraren** i resultatlistan. På fliken **Processer** under **Namn** högerklickar du på **Utforskaren** och klickar sedan på **Starta om**.
