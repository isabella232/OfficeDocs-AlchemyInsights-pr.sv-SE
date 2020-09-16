---
title: Felsöka OneDrive-krascher
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665016"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="6157e-102">Felsöka OneDrive-krascher</span><span class="sxs-lookup"><span data-stu-id="6157e-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="6157e-103">Om OneDrive kraschar upprepade gånger kan du försöka med följande fel söknings steg:</span><span class="sxs-lookup"><span data-stu-id="6157e-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="6157e-104">**Kontrol lera att register nycklar inte är inställda:**</span><span class="sxs-lookup"><span data-stu-id="6157e-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="6157e-105">Använd Registereditorn och navigera till HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="6157e-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="6157e-106">Om DisableFileSyncNGSC finns och är 1 öppnar du den och ändrar värdet till 0.</span><span class="sxs-lookup"><span data-stu-id="6157e-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="6157e-107">Starta OneDrive manuellt genom att gå till Start</span><span class="sxs-lookup"><span data-stu-id="6157e-107">Manually launch OneDrive by going to Start</span></span> ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6157e-109">, skriv OneDrive i sökrutan och klicka sedan på OneDrive-programmet.</span><span class="sxs-lookup"><span data-stu-id="6157e-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6157e-110">**Återställ OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="6157e-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="6157e-111">Kommentarer:</span><span class="sxs-lookup"><span data-stu-id="6157e-111">Notes:</span></span>

- <span data-ttu-id="6157e-112">Om du återställer OneDrive kopplas alla befintliga synkroniseringskopplingar (inklusive ditt personliga OneDrive om det är konfigurerat).</span><span class="sxs-lookup"><span data-stu-id="6157e-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="6157e-113">Du förlorar inte filer eller data genom att återställa OneDrive på datorn.</span><span class="sxs-lookup"><span data-stu-id="6157e-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="6157e-114">**Så här återställer du OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="6157e-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="6157e-115">Öppna dialog rutan Kör genom att trycka på Windows-tangenten och R.</span><span class="sxs-lookup"><span data-stu-id="6157e-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="6157e-116">Skriv% localappdata% \Microsoft\OneDrive\onedrive.exe/reset. och klicka på OK.</span><span class="sxs-lookup"><span data-stu-id="6157e-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="6157e-117">Ett kommando fönster kan komma att visas kort.</span><span class="sxs-lookup"><span data-stu-id="6157e-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="6157e-118">Starta OneDrive manuellt genom att gå till Start</span><span class="sxs-lookup"><span data-stu-id="6157e-118">Manually launch OneDrive by going to Start</span></span> ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6157e-120">, skriv OneDrive i sökrutan och klicka sedan på OneDrive-programmet.</span><span class="sxs-lookup"><span data-stu-id="6157e-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6157e-121">Kommentarer:</span><span class="sxs-lookup"><span data-stu-id="6157e-121">Notes:</span></span>

- <span data-ttu-id="6157e-122">Om du inte har valt att synkronisera vissa mappar före återställningen måste du göra det när synkroniseringen är klar.</span><span class="sxs-lookup"><span data-stu-id="6157e-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="6157e-123">Läsa [Välj vilka OneDrive-mappar som ska synkroniseras med din dator](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   för mer information.</span><span class="sxs-lookup"><span data-stu-id="6157e-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="6157e-124">Du måste slutföra detta för din personliga OneDrive och OneDrive för företag.</span><span class="sxs-lookup"><span data-stu-id="6157e-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>