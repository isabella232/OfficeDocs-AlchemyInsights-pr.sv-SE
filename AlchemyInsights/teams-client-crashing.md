---
title: Teams klient kraschar
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
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321643"
---
# <a name="teams-client-crashing"></a>Teams klient kraschar

Om Teams-klienten kraschar kan du prova följande:

- Om du använder skrivbordsversionen av Teams kan du [kontrollera att programmet är helt uppdaterat](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Kontrollera att alla [Microsoft 365 URL:er och adressintervall](https://docs.microsoft.com/microsoftteams/connectivity-issues) är tillgängliga.

- Logga in med ditt klientadministratörskonto och kontrollera [hälsoinstrumentpanelen](https://docs.microsoft.com/office365/enterprise/view-service-health) för att verifiera att det inte finns något avbrott eller försämrad tjänst.

- Avinstallera och installera om Teams program
    - Bläddra till mappen %appdata%\Microsoft\Teams\ på datorn och ta bort alla filer i katalogen.
    - [Ladda ned och](https://www.microsoft.com/microsoft-teams/download-app)installera Teams-appen och installera om möjligt Teams som administratör (högerklicka på Teams-installationsprogrammet och välj Kör som administratör om det **finns).**

Om din Teams-klient fortfarande kraschar försöker du att återskapa problemet. Om du kan:

1. Använd Steps Recorder för att spela in dina steg.
    - Stäng alla onödiga eller konfidentiella program.
    - Starta Steps Recorder och återskapa problemet när du är inloggad med det aktuella användarkontot.
    - [Samla in de teamloggar som avbildar de inspelade återpropro-stegen](https://docs.microsoft.com/microsoftteams/log-files). 
    
    **Obs!** Se till att du registrerar inloggningsadressen för den påverkade användaren.
    - Samla in information om avdump och/eller fel bucket (Windows). Starta Windows Powershell på den dator där kraschen inträffar och kör följande kommandon (tryck på Retur efter varje kommando):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. När textfilen har genererats och visas på skärmen sparar du filen och bifogar den till tjänstbegäran. 
