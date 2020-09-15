---
title: Felsöka problem med att registrera Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658896"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Felsöka problem med att registrera Windows-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
Vanliga fel meddelanden och lösnings steg:
  
 **Det gick inte att installera program varan, 0x80cf4017:** Ditt konto certifikat har upphört att gälla. Ladda ner om klient program varu paketet för PC client i Intune-administratörskonsolen. Mer information finns i den här dokumentationen.
  
 **Felkod 0x801c0003:** Felet kan uppstå i följande scenarier:
  
-  Användaren har fler enheter registrerade än enhets gränsen. Granska dessa dokument för att [ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [Ändra enhetens gräns](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Användare kan ansluta enheter till Azure AD" är inställt på "ingen". Ange den till alla eller Välj användare. Mer information finns i [den här dokumentationen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Enheten har redan registrerats av en annan användare. Om så är fallet, ta bort enheten från Azure Intune-konsolen eller avregistrera enheten manuellt innan du försöker igen.

-  Enheten är Windows 10 Home. Endast Windows 10 Pro, utbildning och företags-SKU: er kan ansluta till Azure Active Directory.

Ytterligare resurser för att lösa problemet:
  
-  Använd [fel söknings portalen för Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnosticera och lösa vanliga registrerings problem. Granska [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

-  Granska de här dokumenten för en lista över vanliga fel som kan förhindra registrering och problemlösning för var och en av dem: [fel söknings guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) och [fel söknings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Lär dig hur du registrerar Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
