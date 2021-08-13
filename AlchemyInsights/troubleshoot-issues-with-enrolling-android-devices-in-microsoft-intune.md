---
title: Felsöka problem med registrering av Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008096"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Felsöka problem med registrering av Android-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
Några vanliga problem och lösningssteg:
  
 **Felet Enheten är inte krypterad i Företagsportal:** Nyare versioner av Android, särskilt från och med v7.0, kräver ett lösenord för start så att enheten är fullständigt krypterad. Vanliga lösningar är att aktivera en startkod eller kryptera enheten helt och hållet. Mer information [finns i](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) det här dokumentet.
  
 **Enheter kan inte checka in med Intune-tjänsten eller visas som "Ej fel" i Intune-administratörskonsolen:** Vissa Samsung 4.4- och 5.5-enheter kanske inte checkar in tjänsten. Det finns 3 möjliga lösningar på det här problemet:
  
1. Öppna appen Intune-företagsportal, vilket automatiskt initierar en enhetssynkronisering.

2. Uppdatera enheten till Android 6.0 eller senare.

3. Inaktivera Samsung Smart Manager från att hantera Intune-företagsportal. Läs [det här dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) om du vill ha mer information om dessa problem och lösningar.

 **Felet Ogiltig användarlicenstyp** **eller Namn identifieras inte:** Användaren måste tilldelas en Intune- eller EMS-licens. Läs dessa dokument om du vill tilldela en licens via: Office Admin Center eller Azure Portal.
  
Ytterligare resurser som kan hjälpa dig att lösa problemet:
  
1. Använd [Intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.

2. I [det här dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en.

3. [Lär dig hur du registrerar Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
