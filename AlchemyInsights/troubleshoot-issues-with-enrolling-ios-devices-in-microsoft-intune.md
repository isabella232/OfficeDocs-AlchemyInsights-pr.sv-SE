---
title: Felsöka problem med att registrera iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736176"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Felsöka problem med att registrera iOS-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu. 
  
Några vanliga felmeddelanden och lösningssteg:
  
- **Enhetslocket nått** Användaren har fler enheter registrerade än enhetsgränsen. Granska dessa dokument om du vill [ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller ändra [enhetsgränsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Den här tjänsten stöds inte. Ingen registreringspolicy:** Apple Push Notification Service (APNS) måste konfigureras eller förnyas. Läs [det här dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) för instruktioner om hur du gör det. 
    
- **Ogiltig användarlicenstyp eller användarnamnet känns inte igen:** Användaren måste tilldelas en Intune- eller EMS-licens. Granska dessa dokument för att tilldela en licens via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller Azure [Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Ytterligare resurser som hjälper dig att lösa problemet:
  
1. Använd [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information. 
    
2. Granska dessa dokument för en lista över vanliga fel som förhindrar registrering och lösningar till varje: [Felsökningsguide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) och [Felsökningsdokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Läs om hur du registrerar iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

