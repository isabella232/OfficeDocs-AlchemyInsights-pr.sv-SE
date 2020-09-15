---
title: Felsöka problem med registrering av Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689972"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Felsöka problem med registrering av Android-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
Några vanliga problem och problemlösning:
  
 **Enheten är inte krypterad fel i företags portalen:** Nyare versioner av Android, särskilt från och med v 7.0, kräver ett start program för att kontrol lera att enheten är fullständigt krypterad. Vanliga lösningar är att aktivera en start-PIN-kod eller helt kryptera enheten. Granska [det här dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) för mer information.
  
 **Enheter kan inte checka in med Intune-tjänsten eller Visa som "ohälsosamy" i Intune-administratörskonsolen:** Vissa Samsung 4,4-och 5,5-enheter kanske inte checkar in tjänsten. Det finns tre möjliga lösningar på det här problemet:
  
1. Öppna programmet Intune-företagsportalsappen manuellt, som automatiskt initierar en synkronisering.

2. Uppdatera enheten till Android 6,0 eller högre.

3. Inaktivera den smarta hanteraren för Samsung från att hantera Intune-företagsportalsappen. Granska [det här dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) om du vill ha mer information om dessa problem och lösningar.

 **Användar licens typen är ogiltig** eller **användar namnet känns inte igen:** användaren måste tilldelas en Intune-eller EMS-licens. Granska dessa dokument om du vill tilldela en licens via: administrations Center för Office eller Azure Portal.
  
Ytterligare resurser för att lösa problemet:
  
1. Använd [fel söknings portalen för Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnosticera och lösa vanliga registrerings problem. Granska [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

2. Granska [det här dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) för en lista över vanliga fel som kan förhindra registrering och upplösningar till var och en.

3. [Lär dig att registrera Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
