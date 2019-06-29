---
title: Felsöka problem med att registrera Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367307"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Felsöka problem med att registrera Android-enheter i Microsoft Intune

Granska resurserna i listan nedan för att åtgärda problemet nu.
  
Vissa vanliga problem och stegen:
  
 **Enhet krypteras inte fel i företagets Portal:** Nyare versioner av Android, särskilt från och med v7.0, kräver en start-kod för att kontrollera att enheten är helt krypterad. Gemensamma lösningar är att aktivera en start-PIN-kod eller helt kryptera enheten. Granska [dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) för mer information.
  
 **Enheter misslyckas att checka in med tjänsten Intune eller visas som ”ohälsosamt” i Intune-administratörskonsolen:** Vissa Samsung 4.4 och 5.5 enheter kan inte checka in i tjänsten. Det finns 3 möjliga lösningar på problemet:
  
1. Öppna appen Intune-företagsportal som kommer automatiskt att starta en enhetssynkronisering manuellt.

2. Uppdatera enheten till Android 6.0 eller senare.

3. Inaktivera Samsung Smart Manager från att hantera Intune-företagsportal. Granska [dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) för mer information om dessa problem och lösningar.

 **Ogiltig användare licens typ** eller **användare namn inte identifieras fel:** användaren måste tilldelas en Intune eller EMS-licens. Granska dessa dokument om du vill tilldela en licens till: Office Admin Center eller Azure portal.
  
Ytterligare resurser för att lösa problemet:
  
1. Du kan använda [Intune felsökning Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och åtgärda vanliga fel i anmälan. Granska [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

2. Granska [dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) för en lista över vanliga fel som förhindrar registrering och lösningar till varje.

3. [Lär dig att registrera Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
