---
title: Felsöka problem med att registrera iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507021"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Felsöka problem med att registrera iOS-enheter i Microsoft Intune

Granska resurserna som anges nedan för att lösa problemet nu. 
  
Några vanliga felmeddelanden och Lösningssteg:
  
- **Enhets locket har uppnåtts** Användaren har fler enheter registrerade än enhets gränsen. Granska dessa dokument för att [ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [ändra enhets gränsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Den här tjänsten stöds inte. Ingen registreringsprincip:** Apple Push Notification Service (APNS) måste konfigureras eller förnyas. Läs igenom [det här dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) för instruktioner om hur du gör det. 
    
- **Användarlicenstyp ogiltig eller användarnamn känns inte igen:** Användaren måste tilldelas en Intune-eller EMS-licens. Granska dessa dokument för att tilldela en licens via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ytterligare resurser som hjälper dig att lösa problemet:
  
1. Använd [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs igenom [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information. 
    
2. Granska de här dokumenten för en lista över vanliga fel som förhindrar registrering och upplösningar för varje: [felsökningsguide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [Felsökning](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)av dokument.
    
3. [Lär dig hur du registrerar iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

