---
title: Felsöka problem med registrering av iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708980"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Felsöka problem med registrering av iOS-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu. 
  
Några vanliga felmeddelanden och lösningssteg:
  
- **Enhetens änd cap har nåtts** Användaren har fler enheter registrerade än enhetsgränsen. Granska dessa dokument om [du vill ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller ändra [enhetsgränsen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Den här tjänsten stöds inte. Ingen registreringspolicy:** Apple Push-aviseringstjänsten (APNS) måste konfigureras eller förnyas. I [det här dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) finns anvisningar om hur du gör det. 
    
- **Användarlicenstyp ogiltig eller användarnamnet identifieras inte:** Användaren måste vara tilldelad en Intune- eller EMS-licens. Granska de här dokumenten om du vill tilldela en licens via: [Administrationscenter för Office](https://docs.microsoft.com/intune/licenses-assign) [eller Azure Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Ytterligare resurser som kan hjälpa dig att lösa problemet:
  
1. Använd [intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsproblem. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information. 
    
2. I de här dokumenten finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en: [Felsökningsguide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [felsökningsdokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Lär dig hur du registrerar iOS-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

