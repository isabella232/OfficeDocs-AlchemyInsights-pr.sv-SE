---
title: Felsöka problem med att registrera Windows enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981059"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Felsöka problem med att registrera Windows enheter i Microsoft Intune

Granska resurserna nedan för att lösa problemet nu.
  
Några vanliga felmeddelanden och lösningssteg:
  
 **Programvaran kan inte installeras på följande 0x80cf4017:** Ditt kontocertifikat har upphört att gälla. Ladda ned pc-klientprogramvaran igen i Intune-administratörskonsolen. Mer information finns i den här dokumentationen.
  
 **Felkod 0x801c0003:** Felet kan uppstå i följande scenarier:
  
-  Användaren har fler enheter registrerade än enhetsgränsen. Läs dessa dokument om du [vill ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller ändra [enhetsgränsen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Användare kan gå med i enheter till Azure AD" är inställt på "ingen". Ställ in den på alla eller välj användare. Mer information [finns i](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) den här dokumentationen.

-  Enheten har redan registrerats av en annan användare. I så fall tar du bort enheten från Azure Intune-konsolen eller avregistrerar manuellt enheten innan du försöker igen.

-  Enheten är Windows 10 Home. Det är Windows 10 Pro företag-, utbildnings- och utbildnings-SKU:er som kan gå med i Azure Active Directory.

Ytterligare resurser som kan hjälpa dig att lösa problemet:
  
-  Använd [Intune-felsökningsportalen](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och lösa vanliga registreringsfel. Läs [det här dokumentet](https://docs.microsoft.com/intune/help-desk-operators) om du vill ha mer information.

-  I de här dokumenten finns en lista över vanliga fel som förhindrar registrering och upplösning till var och en: [Felsökningsguide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) och [Felsökningsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Lär dig hur du registrerar Windows enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
