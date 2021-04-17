---
title: DataProtection – Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 8166a055d7a967faab83484619b443cc98239c7c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815633"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivera Bitlocker-kryptering med Intune

Intune Endpoint Protection Policy kan användas för att konfigurera Bitlocker-krypteringsinställningar för Windows-enheter. Mer information finns i [Windows 10-inställningar (och senare) för att skydda enheter med Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Utöver Endpoint Protection-policyn finns det även en krypteringsrapport som ger en mer detaljerad vy av krypteringsstatusen för enheter. Du kommer åt den här rapporten från MEM-portalen under **Enheter > Bildskärm** och under Konfiguration **väljer** du sedan [Krypteringsrapport](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Om du upptäcker att Bitlocker inte kan aktiveras som förväntat eller att den profil som används för att aktivera BitLocker är felaktig kan du läsa krypteringsrapporten för att få en bättre förståelse av varför beteendet inträffar.

Mer information om hur du tolkar rapporten, inklusive olika statusvärden för kryptering, finns i Övervaka [enhetskryptering med Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Du bör vara medveten om att många nyare enheter som kör Windows 10 stöder automatisk BitLocker-kryptering som utlöses utan tillämpning av MDM-policy. Det kan påverka tillämpning av principen om inställningar som inte är standard konfigureras. Mer information finns i vanliga frågor och svar.

Mer information om felsökning av bitlocker-problem finns [i Felsöka BitLocker-principer i Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**FAQ**

F: Vilka versioner av Windows stöder enhetskryptering med hjälp av Endpoint Protection Policy?<br>
S: Inställningarna i Intune Endpoint Protection Policy implementeras med [Bitlocker CSP.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Alla versioner av Windows stöder inte Bitlocker-CSP. <br><br>

F: Hur kan Bitlocker aktiveras på enheter utan interaktion med slutanvändare?<br>
S: Så länge alla nödvändiga förutsättningar uppfylls går det att aktivera Bitlocker "Silent Encryption" via Intune. Läs mer om enhetskrav och exempelprincipinställningar för att aktivera tyst kryptering i följande dokument: [Tyst aktivera Bitlocker-kryptering](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

F: Om en enhet redan är krypterad med Bitlocker med standardinställningarna för operativsystem för krypteringsmetod och chifferstyrka (XTS-AES-128) tillämpas en princip med olika inställningar automatiskt för att omkryptera enheten med de nya inställningarna?<br>
S: nej. För att de nya inställningarna för chiffer ska användas måste enheten först dekrypteras.<br><br>
**Obs!** För enheter som registreras med Autopilot utlöses inte den automatiska krypteringen som skulle ske under OOBE förrän Intune-principen har utvärderats, så att de principbaserade inställningarna kan användas i stället för operativsystemets standardinställningar.
 
F: Om en enhet krypteras som ett resultat av programmet för Intune-principen, kommer den att dekrypteras när den principen tas bort?<br>
S: Borttagning av krypteringsrelaterad princip leder INTE till dekryptering av enheter som har konfigurerats.
 
F: Varför visar Intune-efterlevnadsprincipen att min enhet inte har Bitlocker aktiverat, trots att den är det?<br>
S: Inställningen "Bitlocker aktiverad" i Intune-efterlevnadsprincipen använder Klienten WINDOWS Device Health Attestation (GENI). Den här klienten mäter endast enhetens status vid starttid. Så om en enhet inte har startats om sedan Bitlocker-krypteringen slutfördes rapporterar INTE CLIENT-klienttjänsten Bitlocker som aktiv.
 
 