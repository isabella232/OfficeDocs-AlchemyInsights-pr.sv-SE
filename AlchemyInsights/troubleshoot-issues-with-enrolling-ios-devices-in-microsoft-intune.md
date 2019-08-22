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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507021"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Felsöka problem med att registrera iOS-enheter i Microsoft Intune

Granska resurserna i listan nedan för att åtgärda problemet nu. 
  
Vissa vanliga felmeddelanden och stegen:
  
- **Enheten Cap uppnåtts** Användaren har fler enheter som registrerats än gränsen för enheten. Granska dessa dokument om du vill [Ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [Ändra gränsen för enheten](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Den här tjänsten stöds inte. Ingen registreringsprincip:** Apple Push Notification Service (APNS) måste konfigureras eller förnyas. Granska [dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) för instruktioner om hur du ska göra. 
    
- **Felaktig user License eller okänt användarnamn:** Användaren måste tilldelas en Intune eller EMS-licens. Granska dessa dokument om du vill tilldela en licens till: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ytterligare resurser för att lösa problemet:
  
1. Du kan använda [Intune felsökning Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och åtgärda vanliga fel i anmälan. Granska [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information. 
    
2. Granska dokumenten för en lista över vanliga fel som förhindrar registrering och lösningar till varje: [guide för felsökning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [Felsökning doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Lär dig att registrera iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

