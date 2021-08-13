---
title: Batteriet laddas inte
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
- "9002952"
- "5654"
ms.openlocfilehash: 6d072e4be2465c7744c0862b8b3e755274f3b03d0d6058c0c9f7bf23bef8abbd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979547"
---
# <a name="battery-wont-charge"></a>Batteriet laddas inte

Kontrollera först att anslutningarna är säkra. Vi rekommenderar starkt att du endast använder äkta Microsoft-licensierade nätaggregat.

Därefter kan du försöka stänga av din Surface och ladda den i minst 30 minuter. Starta den sedan igen för att se om det löste problemet.

**Kopplad till ett vägguttag, men det laddar inte**

Om batteriikonen i aktivitetsfältet visar **Ansluten, laddar inte**, så innebär det att Surface har upptäckt strömförsörjningen men att den inte laddar batteriet. Surface kan stängas av när du drar ur sladden. Prova det här:

1. Anslut din Surface till ett vägguttag.
2. Välj sökrutan i aktivitetsfältet, skriv **enhetshanteraren** och välj sedan **Enhetshanteraren** i resultatlistan.
3. Klicka på pilen bredvid kategorin **Batteri**.
4. Dubbeltryck eller dubbelklicka på **Microsoft Surface ACPI-Compliant Control Method Battery**, välj fliken **Drivrutin** och klicka på **Avinstallera > OK**.
5. Välj datorn högst upp i alla kategorier, välj **Åtgärdsmeny** och klicka sedan på **Sök efter maskinvaruändringar**.
6. Låt Surface vara ansluten.

När du har tagit bort batteridrivrutinen installerar du uppdateringarna för Surface och Windows. Mer information finns i [Uppdatera inbyggd programvara för Surface och Windows 10](https://support.microsoft.com/help/4023505). Kontrollera batteriet. Om problemen kvarstår [Framtvinga en avstängning och starta om Surface](https://support.microsoft.com/help/4036280/surface-force-a-shut-down-and-restart-your-surface).

**Mer felsökningsinformation**

LED-lampan ska vara på när strömkontakten är ansluten till Surface-enheten. Om den är inaktiverad, blinkar eller blinkar vitt kan du läsa [Vad du kan göra om strömkontakten eller laddaren till Surface inte fungerar](https://support.microsoft.com/help/4484763/surface-fix-issues-with-your-power-supply). 

Om du har problem med din Surface Book kontrollerar du att skärmen är helt ansluten till tangentbordet. Om den fortfarande inte vill ladda tar du bort skärmen och rensar kopplingarna med ett radergummi. Rengör även stiften på den långa, smala delen av laddaren som du ansluter till din Surface och se till att nålarna är torra.

Om du vill se fler sätt att felsöka batteriproblem kan du läsa[ Surface-batteriet laddar inte eller Surface körs inte på batteri](https://support.microsoft.com/help/4023536/surface-surface-battery-wont-charge).
