---
title: Felsöka problem med registrering av iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047994"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Felsöka problem med registrering av iOS-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu. 
  
Några vanliga felmeddelanden och lösningssteg:
  
- **Enhetens änd cap har nåtts** Användaren har fler enheter registrerade än enhetsgränsen. Läs dessa dokument om du [vill ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller ändra [enhetsgränsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Den här tjänsten stöds inte. Ingen registreringspolicy:** Apple Push Notification Service (APNS) måste konfigureras eller förnyas. Läs [det här dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) för anvisningar om hur du gör det. 
    
- **Användarlicenstyp Ogiltig eller Användarnamnet har inte identifierats:** Användaren måste tilldelas en Intune- eller EMS-licens. Läs dessa dokument om du vill tilldela en licens via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller Azure [Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ytterligare resurser som kan hjälpa dig att lösa problemet:
  
1. Använd [Intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information. 
    
2. I de här dokumenten finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en: [Felsökningsguide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [Felsökningsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Lär dig hur du registrerar iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

