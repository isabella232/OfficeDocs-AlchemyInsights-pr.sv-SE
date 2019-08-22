---
title: Felsöka problem med att registrera Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559679"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Felsöka problem med att registrera Windows-enheter i Microsoft Intune

Granska resurserna i listan nedan för att åtgärda problemet nu.
  
Vissa vanliga felmeddelanden och stegen:
  
 **Går inte att installera programvaran, 0x80cf4017:** Konto-certifikatet har upphört att gälla. Hämta igen programpaketet PC-klient i Intune-administratörskonsolen. Läs dokumentationen för mer information.
  
 **Felkod 0x801c0003:** Felet kan uppstå i följande scenarier:
  
1. Användaren har fler enheter som registrerats än gränsen för enheten. Granska dessa dokument om du vill [Ta bort en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [Ändra gränsen för enheten](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. ”Användare kan ansluta enheter till Azure AD” anges till ”none”. Ange alla eller Välj användare. Läs [dokumentationen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) för mer information.

3. Enheten är redan registrerats av en annan användare. Om så är fallet, ta bort enheten från konsolen Azure Intune eller unenroll enheten manuellt innan du försöker igen.

4. Enheten är Windows 10 Home. Endast Windows 10 Pro, utbildning och Enterprise SKU: er kan ansluta till Azure Active Directory.

Ytterligare resurser för att lösa problemet:
  
1. Du kan använda [Intune felsökning Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) för att diagnostisera och åtgärda vanliga fel i anmälan. Granska [dokumentet](https://docs.microsoft.com/intune/help-desk-operators) för mer information.

2. Granska dokumenten för en lista över vanliga fel som förhindrar registrering och lösningar till varje: [guide för felsökning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) och [Felsökning doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Lär dig hur du registrerar Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
