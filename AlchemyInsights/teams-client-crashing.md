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
# <a name="teams-client-crashing"></a><span data-ttu-id="18a5f-102">Kraschar Teams-klienten?</span><span class="sxs-lookup"><span data-stu-id="18a5f-102">Teams client crashing?</span></span>

<span data-ttu-id="18a5f-103">Om Teams-klienten kraschar kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="18a5f-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="18a5f-104">Om du använder skrivbordsversionen av Teams kan du [kontrollera att programmet är helt uppdaterat](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="18a5f-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="18a5f-105">Kontrollera att alla [URL:er och adressintervall för Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) är tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="18a5f-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="18a5f-106">Logga in med ditt klientadministratörskonto och kontrollera hälsoinstrumentpanelen för att verifiera att det inte finns något avbrott eller försämrad tjänst. [](https://docs.microsoft.com/office365/enterprise/view-service-health)</span><span class="sxs-lookup"><span data-stu-id="18a5f-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="18a5f-107">Avinstallera och installera om Teams-programmet (länk)</span><span class="sxs-lookup"><span data-stu-id="18a5f-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="18a5f-108">Bläddra till mappen %appdata%\Microsoft\teams\ på datorn och ta bort alla filer i katalogen.</span><span class="sxs-lookup"><span data-stu-id="18a5f-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="18a5f-109">[Ladda ned och installera Teams-appen](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)och installera om möjligt Teams som administratör (högerklicka på Teams-installationsprogrammet och välj Kör som administratör om det finns).</span><span class="sxs-lookup"><span data-stu-id="18a5f-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="18a5f-110">Kan du återskapa problemet om Teams-klienten fortfarande kraschar?</span><span class="sxs-lookup"><span data-stu-id="18a5f-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="18a5f-111">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="18a5f-111">If so:</span></span>

1. <span data-ttu-id="18a5f-112">Använd Steps Recorder för att spela in dina steg.</span><span class="sxs-lookup"><span data-stu-id="18a5f-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="18a5f-113">Stäng alla onödiga eller konfidentiella program.</span><span class="sxs-lookup"><span data-stu-id="18a5f-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="18a5f-114">Starta Steps Recorder och återskapa problemet när du är inloggad med det aktuella användarkontot.</span><span class="sxs-lookup"><span data-stu-id="18a5f-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="18a5f-115">[Samla in de teamloggar som avbildar de inspelade återpropro-stegen](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="18a5f-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="18a5f-116">**Obs!** Se till att du registrerar inloggningsadressen för den påverkade användaren.</span><span class="sxs-lookup"><span data-stu-id="18a5f-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="18a5f-117">Samla in information om avdump och/eller fel bucket (Windows).</span><span class="sxs-lookup"><span data-stu-id="18a5f-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="18a5f-118">Starta Windows Powershell på den dator där kraschen inträffar och kör följande kommandon:</span><span class="sxs-lookup"><span data-stu-id="18a5f-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="18a5f-119">Bifoga filen till ditt supportfall.</span><span class="sxs-lookup"><span data-stu-id="18a5f-119">Attach the file to your support case.</span></span>
