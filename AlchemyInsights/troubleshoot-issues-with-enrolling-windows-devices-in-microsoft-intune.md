---
title: Felsöka problem med registrering av Windows-enheter i Microsoft Intune
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
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708908"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Felsöka problem med registrering av Windows-enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
Några vanliga felmeddelanden och lösningssteg:
  
 **Programvaran kan inte installeras på följande 0x80cf4017:** Ditt kontocertifikat har upphört att gälla. Ladda ned programvarupaketet för datorklienten igen i Intune-administratörskonsolen. Mer information finns i den här dokumentationen.
  
 **Felkod 0x801c0003:** Felet kan uppstå i följande scenarier:
  
-  Användaren har fler enheter registrerade än enhetsgränsen. Granska dessa dokument om [du vill ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller ändra [enhetsgränsen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Användare kan ansluta enheter till Azure AD" är inställt på "ingen". Ställ in den på alla eller välj användare. Mer information [finns i](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) den här dokumentationen.

-  Enheten har redan registrerats av en annan användare. I så fall tar du bort enheten från Azure Intune-konsolen eller avmarkerar manuellt enheten innan du försöker igen.

-  Enheten är Windows 10 Home. Endast Windows 10 Pro-, Education- och Enterprise-SKU:er kan ansluta till Azure Active Directory.

Ytterligare resurser som kan hjälpa dig att lösa problemet:
  
-  Använd [intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsproblem. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.

-  I de här dokumenten finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en: [Felsökningsguide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) och [felsökningsdokument.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Lär dig hur du registrerar Windows-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
