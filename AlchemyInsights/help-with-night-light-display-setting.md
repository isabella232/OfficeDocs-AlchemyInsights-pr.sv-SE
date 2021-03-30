---
title: Hjälp med inställningen för nattlampan
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405182"
---
# <a name="help-with-the-night-light-display-setting"></a>Hjälp med inställningen för nattlampan

Mer information om bildskärmsinställningar för natttid finns [i Ställ in bildskärmen på natttid i Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Om alternativen för nattljus är nedtonade i Inställningar kontrollerar du bildskärmsdrivrutinen: 

1. Klicka på sökrutan i Aktivitetsfältet, **skriv Enhetshanteraren** och välj **sedan Enhetshanteraren** i sökresultatet.
1. Expandera **Bildskärmskort**. 

Funktionen nattlampan är tyvärr inte tillgänglig om enheten använder en DisplayLink-drivrutin eller en grundläggande bildskärmsdrivrutin.

Nattlampan använder den senaste grafiktekniken så du kan behöva uppdatera bildskärmsdrivrutinen:  

- Sök efter uppdateringar genom att gå till **Starta**  >  **inställningar Uppdatering**&  >  **säkerhetsuppdatering** Windows  >  **Update** Sök  >  **efter uppdateringar.**  

ELLER

- Gå till maskinvarutillverkarens supportwebbplats och ladda ned och installera de senaste bildskärmsdrivrutinerna manuellt.

## <a name="reset-night-light-in-the-registry"></a>Återställa nattlampan i registret

Om det inte fungerar att uppdatera visningsdrivrutinen kan du behöva återställa nattlampan i registret.  

**Varning!** Det här steget för felsökning rekommenderas endast för avancerade användare. Om du ändrar i registret på fel sätt kan det orsaka allvarliga problem. För ytterligare skydd bör du skydda registret innan du ändrar det så att du kan återställa det om det uppstår problem.

1. Skriv **regedit** i sökrutan och välj sedan **Registereditorn** i sökresultatet.

1. Gå till följande registernyckel: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Exportera och ta sedan bort följande undernyckel:$$windows.data.bluelightreduktion.bluelightreduktionsstate

1. Exportera och ta sedan bort följande undernyckel:$$windows.data.bluelightreduktion.settings

1. Starta om Windows och kontrollera om alternativen för nattlampan är tillgängliga.


