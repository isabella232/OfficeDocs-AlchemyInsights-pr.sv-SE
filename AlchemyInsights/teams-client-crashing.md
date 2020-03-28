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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030670"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="18568-102">Kraschar Teams-klienten?</span><span class="sxs-lookup"><span data-stu-id="18568-102">Teams client crashing?</span></span>

<span data-ttu-id="18568-103">Om Teams-klienten kraschar kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="18568-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="18568-104">Om du använder skrivbordsversionen av Teams kan du [kontrollera att programmet är helt uppdaterat](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="18568-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="18568-105">Kontrollera att alla [Office 365-webbadresser och adressintervall](https://docs.microsoft.com/microsoftteams/connectivity-issues) är tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="18568-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="18568-106">Logga in med ditt administratörskonto och kontrollera att det inte finns några avbrott eller prestandaförsämringar i [Instrumentpanel för tjänststatus](https://docs.microsoft.com/office365/enterprise/view-service-health).</span><span class="sxs-lookup"><span data-stu-id="18568-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="18568-107">Som ett sista steg kan du prova att rensa Teams-klientens cache:</span><span class="sxs-lookup"><span data-stu-id="18568-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="18568-108">Avsluta Microsoft Teams-skrivbordsklienten helt.</span><span class="sxs-lookup"><span data-stu-id="18568-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="18568-109">Du kan högerklicka på **Teams** i ikonfältet och klicka på **Avsluta** eller köra aktivitetshanteraren och avsluta processen helt.</span><span class="sxs-lookup"><span data-stu-id="18568-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="18568-110">Gå till Utforskaren och skriv %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="18568-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="18568-111">I katalogen ser du några av följande mappar:</span><span class="sxs-lookup"><span data-stu-id="18568-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="18568-112">I **Programcache** går du till cachen och tar bort alla filer från cacheplatsen: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="18568-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="18568-113">I **Blob_storage** tar du bort alla filer: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="18568-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="18568-114">I **Cache** tar du bort alla filer: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="18568-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="18568-115">I **databaser** tar du bort alla filer: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="18568-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="18568-116">I **GPUCache** tar du bort alla filer: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="18568-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="18568-117">I **IndexedDB** tar du bort .db-filen: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="18568-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="18568-118">I **Lokal lagring** tar du bort alla filer: %appdata%\Microsoft\teams\Local storage.</span><span class="sxs-lookup"><span data-stu-id="18568-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="18568-119">Till sist tar du bort alla filer i **tmp**: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="18568-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="18568-120">Starta om Teams-klienten.</span><span class="sxs-lookup"><span data-stu-id="18568-120">Restart your Teams client.</span></span>
