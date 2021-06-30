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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187739"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="9adf6-102">Teams klient kraschar</span><span class="sxs-lookup"><span data-stu-id="9adf6-102">Teams client crashing</span></span>

<span data-ttu-id="9adf6-103">Om Teams-klienten kraschar kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="9adf6-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="9adf6-104">Om du använder skrivbordsversionen av Teams kan du [kontrollera att programmet är helt uppdaterat](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="9adf6-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="9adf6-105">Kontrollera att alla [Microsoft 365 URL:er och adressintervall](/microsoftteams/connectivity-issues) är tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="9adf6-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="9adf6-106">Logga in med ditt klientadministratörskonto och kontrollera hälsoinstrumentpanelen för att verifiera att det inte finns något avbrott eller försämrad tjänst. [](/office365/enterprise/view-service-health)</span><span class="sxs-lookup"><span data-stu-id="9adf6-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="9adf6-107">Avinstallera och installera om Teams program</span><span class="sxs-lookup"><span data-stu-id="9adf6-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="9adf6-108">Bläddra till mappen %appdata%\Microsoft\Teams\ på datorn och ta bort alla filer i katalogen.</span><span class="sxs-lookup"><span data-stu-id="9adf6-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="9adf6-109">[Ladda ned och installera Teams-appen](https://www.microsoft.com/microsoft-teams/download-app)och installera om möjligt Teams som administratör (högerklicka på Teams-installationsprogrammet och välj Kör som administratör om det **finns).**</span><span class="sxs-lookup"><span data-stu-id="9adf6-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="9adf6-110">Om din Teams-klient ändå kraschar försöker du att återskapa problemet.</span><span class="sxs-lookup"><span data-stu-id="9adf6-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="9adf6-111">Om du kan:</span><span class="sxs-lookup"><span data-stu-id="9adf6-111">If you can:</span></span>

1. <span data-ttu-id="9adf6-112">Använd Steps Recorder för att spela in dina steg.</span><span class="sxs-lookup"><span data-stu-id="9adf6-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="9adf6-113">Stäng alla onödiga eller konfidentiella program.</span><span class="sxs-lookup"><span data-stu-id="9adf6-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="9adf6-114">Starta Steps Recorder och återskapa problemet när du är inloggad med det aktuella användarkontot.</span><span class="sxs-lookup"><span data-stu-id="9adf6-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="9adf6-115">[Samla in de teamloggar som avbildar de inspelade återpropro-stegen](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="9adf6-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="9adf6-116">**Obs!** Se till att du registrerar inloggningsadressen för den påverkade användaren.</span><span class="sxs-lookup"><span data-stu-id="9adf6-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="9adf6-117">Samla in information om avdump och/eller fel bucket (Windows).</span><span class="sxs-lookup"><span data-stu-id="9adf6-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="9adf6-118">Starta Windows Powershell på den dator där kraschen inträffar och kör följande kommandon (tryck på Retur efter varje kommando):</span><span class="sxs-lookup"><span data-stu-id="9adf6-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="9adf6-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="9adf6-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="9adf6-120">När textfilen har genererats och visas på skärmen sparar du filen och bifogar den till tjänstbegäran.</span><span class="sxs-lookup"><span data-stu-id="9adf6-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
