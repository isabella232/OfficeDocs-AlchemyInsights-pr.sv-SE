---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908727"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivera BitLocker-kryptering med Intune

 Intune Endpoint Protection-principen kan användas för att konfigurera BitLocker-krypteringsinställningar för Windows-enheter. Mer information finns i [Windows 10 (och senare) inställningar för att skydda enheter med hjälp av Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Du bör vara medveten om att många nyare enheter som kör Windows 10 stöder automatisk BitLocker-kryptering, som utlöses utan tillämpning av MDM-principen. Detta kan påverka tillämpningen av principen om icke-standardinställningar har konfigurerats. Se följande vanliga frågor och svar för mer information.
 
Information om hur du felsöker problem med BitLocker finns [i Felsöka BitLocker-principer i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Vanliga frågor och svar**

 F: vilka utgåvor av Windows stöder enhetskryptering med hjälp av Endpoint Protection-principen?<br>
 A: inställningarna i Intune Endpoint Protection-principen implementeras med hjälp av [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Inte alla utgåvor eller build-versioner av Windows stöder BitLocker CSP. <br><br>
      För tillfället stöds följande Windows-utgåvor: Enterprise, Education, Mobile, Mobile Enterprise och Professional (build 1809 och senare).
 
F: om en enhet redan är krypterad med BitLocker med hjälp av OS standardinställningarna för krypteringsmetod och cipher styrka (XTS-AES-128), kommer att tillämpa en princip med olika inställningar automatiskt utlösa Omkryptering av enheten med de nya inställningarna?<br>
A: Nej. Om du vill använda de nya cipher-inställningarna måste enheten först dekrypteras.<br><br>
**Anmärkning:** För enheter som registreras med autopilot utlöses inte den automatiska kryptering som skulle inträffa under OOBE förrän Intune-principen utvärderas, vilket gör att principbaserade inställningar kan användas i stället för OPERATIVsystemets standardvärden.
 
F: om en enhet krypteras som ett resultat av tillämpningen av Intune-principen, kommer det att dekrypteras när principen tas bort?<br>
S: borttagning av krypteringsrelaterade principer resulterar inte i dekryptering av enheter som har konfigurerats.
 
F: Varför visar Intune efterlevnadsprincip att min enhet inte har BitLocker aktiverat, även om det är?<br>
A: inställningen "BitLocker aktiverad" i Intune-efterlevnadsprincipen använder Windows Device Health attestering (DHA)-klienten. Den här klienten mäter endast enhetsstatus vid uppstart. Så om en enhet inte har startats om eftersom BitLocker-kryptering slutfördes, DHA client service kommer inte att rapportera BitLocker som aktiv.
 
 