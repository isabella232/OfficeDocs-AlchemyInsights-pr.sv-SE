---
title: Felsöka problem med DEP-registrering i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: e77295f0395919a723dcec1a313ca03154ae59b1bea22bf791f3a0f923cab60d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008276"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Felsöka problem med DEP-registrering i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
1. Om DEP-enheten inte kan registrera och MFA (Multi-Factor Authentication) är aktiverat inaktiverar du MFA. För närvarande stöds inte MFA för DEP-registrering

2. Använd [Intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.

3. I de här dokumenten finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en: [Felsökningsguide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [Felsökning av dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

4. [Lär dig mer om programmet för enhetsregistrering](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
