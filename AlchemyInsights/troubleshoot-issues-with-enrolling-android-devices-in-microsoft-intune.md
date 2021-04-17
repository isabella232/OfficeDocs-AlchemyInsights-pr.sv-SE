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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830960"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Felsöka problem med registrering av Android-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
Några vanliga problem och lösningssteg:
  
 **Felmeddelande om att enheten inte är krypterad i företagsportalen:** Nyare versioner av Android, särskilt från och med v7.0, kräver ett lösenord för start så att enheten är fullständigt krypterad. Vanliga lösningar är att aktivera en startkod eller kryptera enheten helt och hållet. Mer information [finns i](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) det här dokumentet.
  
 **Enheter kan inte checka in med Intune-tjänsten eller visas som "Ej fel" i Intune-administratörskonsolen:** Vissa Samsung 4.4- och 5.5-enheter kanske inte checkar in tjänsten. Det finns 3 möjliga lösningar på det här problemet:
  
1. Öppna appen Intune Company Portal manuellt, som automatiskt initierar en enhetssynkronisering.

2. Uppdatera enheten till Android 6.0 eller senare.

3. Inaktivera Samsung Smart Manager från att hantera Intune-företagsportalen. Läs [det här dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) om du vill ha mer information om dessa problem och lösningar.

 **Felet Ogiltig användarlicenstyp** **eller Namn identifieras inte:** Användaren måste tilldelas en Intune- eller EMS-licens. Läs dessa dokument om du vill tilldela en licens via: Administrationscenter för Office eller Azure Portal.
  
Ytterligare resurser som kan hjälpa dig att lösa problemet:
  
1. Använd [Intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.

2. I [det här dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en.

3. [Lär dig hur du registrerar Android-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
