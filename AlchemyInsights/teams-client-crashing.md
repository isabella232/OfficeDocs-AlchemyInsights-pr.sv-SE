---
title: Kraschar Teams-klienten?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826289"
---
# <a name="teams-client-crashing"></a>Kraschar Teams-klienten?

Om Teams-klienten kraschar kan du prova följande:

- Om du använder skrivbordsversionen av Teams kan du [kontrollera att programmet är helt uppdaterat](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Kontrollera att alla [URL:er och adressintervall för Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) är tillgängliga.

- Logga in med ditt klientadministratörskonto och kontrollera hälsoinstrumentpanelen för att verifiera att det inte finns något avbrott eller försämrad tjänst. [](https://docs.microsoft.com/office365/enterprise/view-service-health)

- Avinstallera och installera om Teams-programmet (länk)
    - Bläddra till mappen %appdata%\Microsoft\teams\ på datorn och ta bort alla filer i katalogen.
    - [Ladda ned och installera Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)och installera om möjligt Teams som administratör (högerklicka på Teams-installationsprogrammet och välj Kör som administratör om det finns).

Kan du återskapa problemet om Teams-klienten fortfarande kraschar? Gör så här:

1. Använd Steps Recorder för att spela in dina steg.
    - Stäng alla onödiga eller konfidentiella program.
    - Starta Steps Recorder och återskapa problemet när du är inloggad med det aktuella användarkontot.
    - [Samla in de teamloggar som avbildar de inspelade återpropro-stegen](https://docs.microsoft.com/microsoftteams/log-files). **Obs!** Se till att du registrerar inloggningsadressen för den påverkade användaren.
    - Samla in information om avdump och/eller fel bucket (Windows). Starta Windows Powershell på den dator där kraschen inträffar och kör följande kommandon:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Bifoga filen till ditt supportfall.
