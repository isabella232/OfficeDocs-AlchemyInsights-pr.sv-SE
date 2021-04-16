---
title: Det går inte att öppna en Office-fil när du dubbelklickar på den
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
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814823"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Det går inte att öppna en Office-fil när du dubbelklickar på den

När du dubbelklickat på en Office-fil kan programmet öppnas men själva filen öppnas inte. Eller så kan du få felmeddelandet: "Ett problem uppstod när kommandot skulle skickas till programmet." Det finns många orsaker till detta, men de två vanligaste lösningarna är:

- Kontrollera att DDE-alternativet är avmarkerat i Excel. Du hittar alternativet genom att skapa en ny arbetsbok och sedan välja **Arkiv eller > Alternativ > Avancerat.** I avsnittet **Allmänt** avmarkerar du **ignorera andra program som använder DDE (Dynamic Data Exchange).**

- Kör en onlinereparation för att återställa standardinställningarna. Klicka på Start-knappen i Windows och sök efter "Kontrollpanelen". Öppna **Kontrollpanelen och** gå till Program **för > Program och funktioner**. Högerklicka sedan på **Microsoft Office [version]** och välj **Ändra > Onlinereparation**.

Om ingen av de här lösningarna fungerar kan du hitta en mer fullständig lista med lösningar i hjälpartikeln, så öppnas den inte när du dubbelklickar [på en Office-fil.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
