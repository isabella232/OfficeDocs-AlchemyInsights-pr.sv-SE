---
title: Felsöka problem med att registrera Android-enheter i Microsoft Intune
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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709016"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Felsöka problem med att registrera Android-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
Några vanliga problem och lösningssteg:
  
 **Fel vid enhetskrypterad kommunikation i företagsportalen:** Nyare versioner av Android, särskilt från och med v7.0, kräver ett lösenord för start för att kontrollera att enheten är fullständigt krypterad. Vanliga lösningar är att aktivera en start-PIN eller kryptera enheten helt. Mer information [finns i](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) det här dokumentet.
  
 **Enheter kan inte checka in med Intune-tjänsten eller visas som "Ej fel" i intune-administratörskonsolen:** Vissa Samsung 4.4- och 5.5-enheter kanske inte checkar in tjänsten. Det finns tre möjliga lösningar på det här problemet:
  
1. Öppna appen Intune-företagsportal manuellt, som automatiskt initierar en enhetssynkronisering.

2. Uppdatera enheten till Android 6.0 eller senare.

3. Inaktivera Samsungs Smart Manager från att hantera Intune-företagsportalen. I [det här dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) finns mer information om dessa problem och lösningar.

 **Felet Ogiltig användarlicenstyp** **eller Användarnamnet identifieras inte:** Användaren måste tilldelas en Intune- eller EMS-licens. Granska dessa dokument för att tilldela en licens via: Administrationscenter för Office eller Azure Portal.
  
Ytterligare resurser som kan hjälpa dig att lösa problemet:
  
1. Använd [intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsproblem. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.

2. I [det här dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en.

3. [Lär dig hur du registrerar Android-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
