---
title: Felsöka problem med att registrera Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665850"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Felsöka problem med att registrera Windows-enheter i Microsoft Intune

Granska resurserna som anges nedan för att lösa problemet nu.
  
Några vanliga felmeddelanden och Lösningssteg:
  
 **Programvaran kan inte installeras, 0x80cf4017:** Ditt kontocertifikat har upphört att gälla. Hämta klientprogram varupaketet för PC på nytt i Intune-administratörskonsolen. Läs igenom den här dokumentationen för mer information.
  
 **Felkod 0x801c0003:** Felet kan uppstå i följande scenarier:
  
-  Användaren har fler enheter registrerade än enhets gränsen. Granska dessa dokument för att [ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [ändra enhets gränsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Användare kan ansluta enheter till Azure AD" är inställt på "none". Ställ in den på alla eller Välj användare. Läs igenom [den här dokumentationen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) för mer information.

-  Enheten har redan registrerats av en annan användare. Om så är fallet, ta bort enheten från Azure Intune-konsolen eller manuellt avregistrera enheten innan du försöker igen.

-  Enheten är Windows 10 Home. Endast Windows 10 Pro, Education och Enterprise SKU: er kan ansluta till Azure Active Directory.

Ytterligare resurser som hjälper dig att lösa problemet:
  
-  Använd [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs igenom [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

-  Granska de här dokumenten för en lista över vanliga fel som förhindrar registrering och upplösningar för varje: [felsökningsguide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) och [Felsökning](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)av dokument.

[Lär dig hur du registrerar Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
