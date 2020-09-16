---
title: Termer saknas i SharePoint Online term lagrings plats
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750469"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivera BitLocker-kryptering med Intune

Intune Endpoint Protection policy kan användas för att konfigurera Boitlocker krypterings inställningar för Windows-enheter enligt beskrivningen i: windows10 (och senare) inställningar för att skydda enheter med Intune

Du bör vara medveten om att många nyare enheter som kör Windows 10 stöder automatisk BitLocker-kryptering som aktive ras utan tillämpning av MDM-princip. Det här kan påverka tillämpningen av policy om icke-standardinställningar konfigureras. Se vanliga frågor för mer information.


Vanliga frågor   Q: vilka versioner av Windows stöder enhets kryptering som använder Endpoint Protection policy?
 A: inställningarna i policyn för Endpoint Protection för Intune implementeras med hjälp av BitLocker-CSP.Alla versioner av Windows stöder inte heller BitLocker-CSP: n. 
      I den här tiden Windows-utgåvor: Enterprise; Utbildning och mobil telefon, mobil telefon och professionellt stöd (från version 1809).




F: om en enhet redan är krypterad med BitLocker med hjälp av OS-standardinställningarna för krypterings metod och chiffrering (XTS-AES-128) tillämpas en princip med olika inställningar automatiskt återaktiverar enheten med de nya inställningarna?

S: nej. För att använda de nya inställningarna för chiffrering måste enheten först dekrypteras.

Anmärkning för enheter som är registrerade med autopilot en automatisk kryptering som skulle inträffa under OOBE utlöses inte förrän Intune-principen utvärderas, vilket gör att principbaserade inställningar används i stället för OS-standardinställningarna




F om en enhet är krypterad som ett resultat av en Intune-princip kommer den att avkrypteras när den principen tas bort?

A: det går inte att dekryptera de enheter som har kon figurer ATS när krypterings relaterad princip tas bort.




F: Varför visas inte min enhet "BitLocker aktive rad" i Intune policy för efterlevnad?

A: inställningen "BitLocker är aktive rad" i Intune policyn använder DHA-klienten (Windows Device Health attestering). Denna klient mäter bara enhetens tillstånd vid start. Om en enhet inte har startats om sedan BitLocker-krypteringen är slutförd, rapporterar inte BitLocker som aktiv.