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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669266"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Felsöka problem med registrering av iOS-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu. 
  
Vanliga fel meddelanden och lösnings steg:
  
- **Höljet har nåtts** Användaren har fler enheter registrerade än enhets gränsen. Granska dessa dokument för att [ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [Ändra enhetens gräns](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Den här tjänsten stöds inte. Ingen registrerings princip:** Apple Push Notification Service (APN) måste konfigureras eller förnyas. Läs [det här dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) för anvisningar om hur du gör det. 
    
- **Användar licens typen är ogiltig eller användar namnet känns inte igen:** Användaren måste tilldelas en Intune-eller EMS-licens. Granska dessa dokument om du vill tilldela en licens via: [administrations Center för Office](https://docs.microsoft.com/intune/licenses-assign) eller [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ytterligare resurser för att lösa problemet:
  
1. Använd [fel söknings portalen för Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnosticera och lösa vanliga registrerings problem. Granska [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information. 
    
2. Granska de här dokumenten för en lista över vanliga fel som kan förhindra registrering och problemlösning för var och en av dem: [fel söknings guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [fel söknings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Lär dig hur du registrerar iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

