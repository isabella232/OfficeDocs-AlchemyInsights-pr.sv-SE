---
title: Felsöka OneDrive-krascher
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826217"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="e5b58-102">Felsöka OneDrive-krascher</span><span class="sxs-lookup"><span data-stu-id="e5b58-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="e5b58-103">Om OneDrive kraschar upprepade gånger kan du prova följande felsökningssteg:</span><span class="sxs-lookup"><span data-stu-id="e5b58-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="e5b58-104">**Kontrollera att registernycklar inte har angetts:**</span><span class="sxs-lookup"><span data-stu-id="e5b58-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="e5b58-105">Med Registereditorn går du till HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="e5b58-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="e5b58-106">Om DisableFileSyncNGSC finns och är inställd på 1 öppnar du nyckeln och ändrar värdet till 0.</span><span class="sxs-lookup"><span data-stu-id="e5b58-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="e5b58-107">Starta OneDrive manuellt genom att gå till Start</span><span class="sxs-lookup"><span data-stu-id="e5b58-107">Manually launch OneDrive by going to Start</span></span> ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e5b58-109">skriver du OneDrive i sökrutan och klickar sedan på OneDrive-skrivbordsprogrammet.</span><span class="sxs-lookup"><span data-stu-id="e5b58-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e5b58-110">**Återställa OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="e5b58-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="e5b58-111">Kommentarer:</span><span class="sxs-lookup"><span data-stu-id="e5b58-111">Notes:</span></span>

- <span data-ttu-id="e5b58-112">Om du återställer OneDrive kopplas alla befintliga synkroniseringsanslutningar bort (inklusive din personliga OneDrive om den är konfigurerad).</span><span class="sxs-lookup"><span data-stu-id="e5b58-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="e5b58-113">Du förlorar inga filer eller data genom att återställa OneDrive på datorn.</span><span class="sxs-lookup"><span data-stu-id="e5b58-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="e5b58-114">**Återställa OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="e5b58-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="e5b58-115">Öppna en dialogruta genom att trycka på Windows-tangenten och R.</span><span class="sxs-lookup"><span data-stu-id="e5b58-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="e5b58-116">Skriv %localappdata%\Microsoft\OneDrive\onedrive.exe /reset och tryck på OK.</span><span class="sxs-lookup"><span data-stu-id="e5b58-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="e5b58-117">Ett kommandofönster kan visas kort.</span><span class="sxs-lookup"><span data-stu-id="e5b58-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="e5b58-118">Starta OneDrive manuellt genom att gå till Start</span><span class="sxs-lookup"><span data-stu-id="e5b58-118">Manually launch OneDrive by going to Start</span></span> ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="e5b58-120">skriver du OneDrive i sökrutan och klickar sedan på OneDrive-skrivbordsprogrammet.</span><span class="sxs-lookup"><span data-stu-id="e5b58-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="e5b58-121">Kommentarer:</span><span class="sxs-lookup"><span data-stu-id="e5b58-121">Notes:</span></span>

- <span data-ttu-id="e5b58-122">Om du har valt att bara synkronisera vissa mappar före återställningen måste du göra det igen när synkroniseringen är klar.</span><span class="sxs-lookup"><span data-stu-id="e5b58-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="e5b58-123">Mer [information finns i Välja vilka OneDrive-mappar som ska synkroniseras](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)på   datorn.</span><span class="sxs-lookup"><span data-stu-id="e5b58-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="e5b58-124">Du måste slutföra detta för din personliga OneDrive och OneDrive för företag.</span><span class="sxs-lookup"><span data-stu-id="e5b58-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>