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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665850"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Felsöka problem med att registrera Windows-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
Några vanliga felmeddelanden och lösningssteg:
  
 **Programvaran kan inte installeras, 0x80cf4017:** Ditt kontocertifikat har upphört att gälla. Ladda ned programvarupaketet för PC-klienten på en ny drivrutin i Intune-administratörskonsolen. Läs den här dokumentationen för mer information.
  
 **Felkod 0x801c0003:** Felet kan uppstå i följande scenarier:
  
-  Användaren har fler enheter registrerade än enhetsgränsen. Granska dessa dokument om du vill [ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller ändra [enhetsgränsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Användare kan ansluta till enheter till Azure AD" är inställt på "ingen". Ställ in den på alla eller välj användare. Läs [den här dokumentationen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) för mer information.

-  Enheten har redan registrerats av en annan användare. Om så är fallet tar du bort enheten från Azure Intune-konsolen eller avregistrerar enheten manuellt innan du försöker igen.

-  Enheten är Windows 10 Home. Endast Windows 10 Pro, Utbildning och Enterprise SKU:er kan ansluta till Azure Active Directory.

Ytterligare resurser som hjälper dig att lösa problemet:
  
-  Använd [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

-  Granska dessa dokument för en lista över vanliga fel som förhindrar registrering och lösningar till varje: [Felsökningsguide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) och [Felsökningsdokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Lär dig hur du registrerar Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
