---
title: Villkor som saknas i SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766871"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivera Bitlocker-kryptering med Intune

Intune Endpoint Protection Policy kan användas för att konfigurera Boitlocker-krypteringsinställningar för Windows-enheter enligt beskrivningen i : Windows10-inställningar (och senare) för att skydda enheter som använder Intune

Du bör vara medveten om att många nyare enheter som kör Windows 10 stöder automatisk bitlockerkryptering som utlöses utan tillämpning av MDM-principen. Detta kan påverka tillämpningen av principen om icke-standardinställningarna är konfigurerade. Se Vanliga frågor och svar för mer information.


Vanliga  frågor och svar F: Vilka versioner av Windows stöder enhetskryptering med hjälp av slutpunktsskyddsprincipen?
 S: Inställningarna i Intune Endpoint Protection Policy implementeras med Bitlocker CSP.Inte alla utgåvor eller versioner av Windows stöder Bitlocker CSP. 
      Vid denna tid Windows Editions: Enterprise; Utbildning, mobil, mobilt företag och professional (från bygg 1809 och framåt) stöds.




F: Om en enhet redan är krypterad med Bitlocker med hjälp av OS-standardinställningarna för krypteringsmetod och chifferstyrka (XTS-AES-128) kommer att tillämpa en princip med olika inställningar automatiskt utlösa omkryptering av enheten med de nya inställningarna?

A: Nej. För att kunna tillämpa de nya chifferinställningarna måste enheten först dekrypteras.

För enheter som registreras med Autopilot utlöses inte den automatiska kryptering som skulle ske under OOBE förrän Intune-principen utvärderas, vilket gör att de principbaserade inställningarna kan användas i stället för OS-standardinställningarna




F Om en enhet krypteras som ett resultat av tillämpningen av Intune-principen kommer den att dekrypteras när den principen tas bort?

S: Borttagning av krypteringsrelaterad princip resulterar INTE i dekryptering av de enheter som har konfigurerats.




F: Varför visar intune Compliance-principen att min enhet inte har "Bitlocker Enabled" men det är?

S: Inställningen "Bitlocker enabled" i intune-efterlevnadsprincipen använder DHA-klienten (Windows Device Health Attestation). Den här klienten mäter endast enhetstillstånd vid uppstart. Så om en enhet inte har startats om sedan bitlocker kryptering slutfördes DHA klienttjänsten kommer inte att rapportera bitlocker som aktiv.