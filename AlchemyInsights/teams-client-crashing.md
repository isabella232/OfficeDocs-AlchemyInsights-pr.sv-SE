---
title: Kraschar Teams-klienten?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354071"
---
# <a name="teams-client-crashing"></a>Kraschar Teams-klienten?

Om Teams-klienten kraschar kan du prova följande:

- Om du använder skrivbordsversionen av Teams kan du [kontrollera att programmet är helt uppdaterat](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Kontrollera att alla [Microsoft 365-url:er och adressintervall](https://docs.microsoft.com/microsoftteams/connectivity-issues) är tillgängliga.

- Logga in med ditt klientadministratörskonto och kontrollera [instrumentpanelen för tjänstens hälsotillstånd](https://docs.microsoft.com/office365/enterprise/view-service-health) för att kontrollera att det inte finns något avbrott eller en tjänstförsämring.

- Avinstallera och installera om Teams Application (länk)
    - Bläddra till mappen %appdata%\Microsoft\teams\ på datorn och ta bort alla filer i katalogen.
    - [Ladda ned och installera Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)och installera om möjligt Teams som administratör (högerklicka på Teams-installationsprogrammet och välj "Kör som administratör" om det är tillgängligt).

Om din Teams-klient fortfarande kraschar, kan du återskapa problemet? Om så är fallet:

1. Använd steginspelaren för att fånga dina steg.
    - Stäng ALLA onödiga eller konfidentiella program.
    - Starta Steps Recorder och återskapa problemet när du är inloggad med det berörda användarkontot.
    - [Samla de teamloggar som fångar de inspelade repro-stegen](https://docs.microsoft.com/microsoftteams/log-files). **Obs:** Se till att du samlar in inloggningsadressen för den påverkade användaren.
    - Samla in information om dump- och/eller felhink (Windows). Starta Windows Powershell på datorn där kraschen inträffar och kör följande kommandon:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Bifoga filen till supportärelet.
