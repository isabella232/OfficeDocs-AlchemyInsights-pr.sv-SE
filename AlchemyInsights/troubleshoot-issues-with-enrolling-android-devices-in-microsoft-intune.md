---
title: Felsöka problem med att registrera Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759638"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Felsöka problem med att registrera Android-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
Några vanliga problem och lösningssteg:
  
 **Enheten har inte krypterat fel i företagsportalen:** Nyare versioner av Android, särskilt från och med v7.0, kräver en startlösenkod för att se till att enheten är helt krypterad. Vanliga lösningar är att aktivera en startstift eller kryptera enheten helt. Läs [det här dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) för mer information.
  
 **Enheter kan inte checka in med Intune-tjänsten eller visas som "Ohälsosam" i Intune-administratörskonsolen:** Vissa Samsung 4.4- och 5.5-enheter kanske inte checkar in på tjänsten. Det finns tre möjliga lösningar på problemet:
  
1. Öppna Intune Company Portal-appen manuellt, som automatiskt initierar en enhetssynkronisering.

2. Uppdatera enheten till Android 6.0 eller senare.

3. Inaktivera Samsung Smart Manager från att hantera Intune Company Portal. Läs [det här dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) för mer information om dessa frågor och lösningar.

 **Fel i användarlicenstypen** Ogiltigt eller **fel som inte känns igen för användarnamn:** Användaren måste tilldelas en Intune- eller EMS-licens. Granska dessa dokument för att tilldela en licens via: Office Admin Center eller Azure-portal.
  
Ytterligare resurser som hjälper dig att lösa problemet:
  
1. Använd [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

2. Granska [det här dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) för en lista över vanliga fel som förhindrar registrering och lösningar till var och en.

3. [Läs om hur du registrerar Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
