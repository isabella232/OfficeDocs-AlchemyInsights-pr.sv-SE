---
title: Felsöka problem med dep-registrering i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 11b0d73c34996fd84431b38d77b64536d386977e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766727"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a>Felsöka problem med dep-registrering i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
1. Om dep-enheten inte kan registrera sig och MFA (Multifaktorautentisering) är aktiverat inaktiverar du MFA. MFA stöds inte för datahederregistrering

2. Använd [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

3. Granska dessa dokument för en lista över vanliga fel som förhindrar registrering och lösningar till var och en: [Felsökningsguide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [felsökningsdokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

4. [Läs mer om programmet för enhetsregistrering](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).
