---
title: Det går inte att Office när du dubbelklickar på en fil
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
ms.openlocfilehash: 519051ac0ffc11d2b17c14959464c1123654bef38d6e10efd252b4ff3d8bbc1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965119"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Det går inte att Office när du dubbelklickar på en fil

När du dubbelklickat Office filen kanske programmet öppnas, men själva filen öppnas inte. Eller så kan du få felmeddelandet: "Ett problem uppstod när kommandot skulle skickas till programmet." Det finns många orsaker till detta, men de två vanligaste lösningarna är:

- I Excel kontrollerar du att DDE-alternativet är avmarkerat. Du hittar alternativet genom att skapa en ny arbetsbok och sedan välja **Arkiv eller > Alternativ > Avancerat.** I avsnittet **Allmänt** avmarkerar du kryssrutan **Ignorera andra program som använder DDE (Dynamic Data Exchange).**

- Kör en onlinereparation för att återställa standardinställningarna. Klicka Windows på Start-knappen och sök efter "Kontrollpanelen". Öppna **Kontrollpanelen och** gå till Program **för > Program och funktioner**. Högerklicka sedan på Microsoft Office **[Version] och** välj **Ändra > Onlinereparation.**

Om ingen av de här lösningarna fungerar kan du hitta en mer fullständig lista med lösningar i supportartikeln, om du dubbelklickar på Office fil inte [öppnar den.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
