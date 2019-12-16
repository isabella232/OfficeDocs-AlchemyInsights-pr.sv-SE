---
title: Termer som saknas i SharePoint Online term Store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053531"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivera BitLocker-kryptering med Intune

Intune Endpoint Protection-principen kan användas för att konfigurera Boitlocker krypteringsinställningar för Windows-enheter som beskrivs i: windows10 (och senare) inställningar för att skydda enheter med hjälp av Intune

Du bör vara medveten om att många nyare enheter som kör Windows 10 stöder automatisk BitLocker-kryptering som utlöses utan tillämpning av MDM-principen. Detta kan påverka tillämpningen av principen om icke-standardinställningar har konfigurerats. Se FAQ för mer information.


FAQ  Q: vilka utgåvor av Windows stöder enhetskryptering med hjälp av Endpoint Protection-principen?
 A: inställningarna i Intune Endpoint Protection-principen implementeras med hjälp av BitLocker CSP.Inte alla utgåvor eller build-versioner av Windows stöder BitLocker CSP. 
      På denna tid Windows upplagor: företag; Education, Mobile, Mobile Enterprise och Professional (från build 1809 och framåt) stöds.




F: om en enhet redan är krypterad med BitLocker med hjälp av OS standardinställningarna för krypteringsmetod och cipher styrka (XTS-AES-128) kommer att tillämpa en princip med olika inställningar automatiskt utlösa Omkryptering av enheten med de nya inställningarna?

A: Nej. För att kunna tillämpa de nya krypteringsinställningarna måste enheten först dekrypteras.

För enheter som registreras med autopilot aktiveras inte den automatiska kryptering som skulle inträffa under OOBE förrän Intune-principen utvärderas, vilket gör att principbaserade inställningar kan användas i stället för OS-standardvärdena




F om en enhet krypteras som ett resultat av tillämpningen av Intune-principen dekrypteras när principen tas bort?

S: borttagning av krypteringsrelaterade principer resulterar inte i dekryptering av enheter som har konfigurerats.




F: Varför visar Intune efterlevnadsprincip att min enhet inte har "BitLocker aktiverat" men det är?

A: inställningen "BitLocker aktiverad" i Intune efterlevnadsprincip använder Windows Device Health attestering (DHA)-klienten. Den här klienten mäter endast enhetsstatus vid uppstart. Så om en enhet inte har startats om eftersom BitLocker-kryptering slutfördes kommer inte DHA client service att rapportera BitLocker som aktiv.