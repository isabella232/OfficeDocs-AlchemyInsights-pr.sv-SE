---
title: Intune Win32 app Deployment
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461994"
---
# <a name="intune-win32-app-deployment"></a>Intune Win32 app Deployment

Microsoft Intune tillåter Win32-program, inklusive men inte begränsat till MSI och. EXE för att distribueras till Windows 10-enheter. Den distributions funktion som används kräver att det finns ett Intune Management Extension (IME) på mål enheten. IME installeras automatiskt som ett resultat av att ett PowerShell-skript eller en Win32-tillämpning distribueras till en användare/enhet.

Det finns också en uppsättning förutsättningar som måste uppfyllas för att du ska kunna distribuera Win32-appar som inkluderar:

- Plattformar som stöds: Windows 10 version 1607 eller senare (Enterprise, Pro och Education-version).
- Arkitektur som stöds: x86 och x64.
- Enhets hantering: AAD-uppkopplad och automatisk registrering (inklusive hybrid domän ansluten och automatisk registrering via grup princip).
- Format för programpaket:. **intunewin**  -fil som skapats av [Microsoft Win32-innehålls förberedelse verktyget](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Begränsat
    - Maximal storlek: 8 GB.
    - Arkitektur som inte stöds: armar.

Granska dokumentet "[Lägg till, tilldela och övervaka en Win32-app i Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" för information som rör dessa steg.

Information om hur du felsöker program distributioner i Windows, inklusive Win32-appar, kan granskas i följande dokument

- [Felsöka problem med programinstallation](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Felsöka Win32-appar](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)