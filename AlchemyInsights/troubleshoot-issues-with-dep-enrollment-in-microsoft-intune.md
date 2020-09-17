---
title: Felsöka problem med DATAEXEKVERINGSSKYDD i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797314"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Felsöka problem med DATAEXEKVERINGSSKYDD i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
1. Om DEP-enheten inte kan registrera och MFA (multifaktorautentisering) är aktive rad måste du inaktivera MFA. För närvarande stöds inte för MFA-registrering

2. Använd [fel söknings portalen för Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnosticera och lösa vanliga registrerings problem. Granska [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

3. Granska dessa dokument för en lista över vanliga fel som kan förhindra registrering och upplösningar på var och en av dem: [fel söknings guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [fel söknings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

4. [Läs mer om programmet för enhets registrering](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
