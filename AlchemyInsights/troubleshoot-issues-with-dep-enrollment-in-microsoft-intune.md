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
ms.openlocfilehash: 3e10f6729d760d9f8f6d04bcb33317fde51a9b80
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507037"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Felsöka problem med Dataexekveringsskydd registrering i Microsoft Intune

Granska resurserna i listan nedan för att åtgärda problemet nu.
  
1. Om Dataexekveringsskyddet enheten går inte att registrera och MFA (autentisering på flera plan) är aktiverad, inaktivera MFA. För närvarande stöds inte MFA för DEP-registrering

2. Du kan använda [Intune felsökning Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och åtgärda vanliga fel i anmälan. Granska [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

3. Granska dokumenten för en lista över vanliga fel som förhindrar registrering och lösningar till varje: [guide för felsökning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [Felsökning doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

4. [Lär dig mer om programmet för registrering av enheten](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
