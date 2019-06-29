---
title: Felsöka problem med Dataexekveringsskydd registrering i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 3df961859cc1e3394ed0e8d779718823ae446d37
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353663"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Felsöka problem med Dataexekveringsskydd registrering i Microsoft Intune

Granska resurserna i listan nedan för att åtgärda problemet nu.
  
1. Om Dataexekveringsskyddet enheten går inte att registrera och MFA (autentisering på flera plan) är aktiverad, inaktivera MFA. För närvarande stöds inte MFA för DEP-registrering

2. Du kan använda [Intune felsökning Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och åtgärda vanliga fel i anmälan. Granska [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

3. Granska dokumenten för en lista över vanliga fel som förhindrar registrering och lösningar till varje: [guide för felsökning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [Felsökning doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

4. [Lär dig mer om programmet för registrering av enheten](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
