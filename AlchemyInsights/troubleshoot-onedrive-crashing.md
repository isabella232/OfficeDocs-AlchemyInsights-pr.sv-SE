---
title: Felsöka OneDrive kraschar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749170"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="6f148-102">Felsöka OneDrive kraschar</span><span class="sxs-lookup"><span data-stu-id="6f148-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="6f148-103">Om OneDrive kraschar flera gånger provar du de här felsökningsstegen:</span><span class="sxs-lookup"><span data-stu-id="6f148-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="6f148-104">**Kontrollera att registernycklarna inte är inställda:**</span><span class="sxs-lookup"><span data-stu-id="6f148-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="6f148-105">Använda Registereditorn och navigera till HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="6f148-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="6f148-106">Om DisableFileSyncNGSC finns och är inställd på 1 öppnar du nyckeln och ändrar värdet till 0.</span><span class="sxs-lookup"><span data-stu-id="6f148-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="6f148-107">Starta OneDrive manuellt genom att gå till Start</span><span class="sxs-lookup"><span data-stu-id="6f148-107">Manually launch OneDrive by going to Start</span></span> ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6f148-109">skriver du OneDrive i sökrutan och klickar sedan på OneDrive-skrivbordsappen.</span><span class="sxs-lookup"><span data-stu-id="6f148-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6f148-110">**Återställa OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="6f148-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="6f148-111">Kommentarer:</span><span class="sxs-lookup"><span data-stu-id="6f148-111">Notes:</span></span>

- <span data-ttu-id="6f148-112">Om du återställer OneDrive kopplas alla befintliga synkroniseringsanslutningar frånkopplad från alla dina befintliga synkroniseringsanslutningar (inklusive din personliga OneDrive om den är konfigurerad).</span><span class="sxs-lookup"><span data-stu-id="6f148-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="6f148-113">Du förlorar inte filer eller data genom att återställa OneDrive på datorn.</span><span class="sxs-lookup"><span data-stu-id="6f148-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="6f148-114">**Så här återställer du OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="6f148-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="6f148-115">Öppna dialogrutan Kör genom att trycka på Windows-tangenten och R.</span><span class="sxs-lookup"><span data-stu-id="6f148-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="6f148-116">Skriv %localappdata%\Microsoft\OneDrive\onedrive.exe /reset och tryck på OK.</span><span class="sxs-lookup"><span data-stu-id="6f148-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="6f148-117">Ett kommandofönster kan visas en kort stund.</span><span class="sxs-lookup"><span data-stu-id="6f148-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="6f148-118">Starta OneDrive manuellt genom att gå till Start</span><span class="sxs-lookup"><span data-stu-id="6f148-118">Manually launch OneDrive by going to Start</span></span> ![Tryck på Windows-tangenten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6f148-120">skriver du OneDrive i sökrutan och klickar sedan på OneDrive-skrivbordsappen.</span><span class="sxs-lookup"><span data-stu-id="6f148-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6f148-121">Kommentarer:</span><span class="sxs-lookup"><span data-stu-id="6f148-121">Notes:</span></span>

- <span data-ttu-id="6f148-122">Om du bara hade valt att synkronisera vissa mappar före återställningen måste du göra det igen när synkroniseringen har slutförts.</span><span class="sxs-lookup"><span data-stu-id="6f148-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="6f148-123">Läs [Välj vilka OneDrive-mappar som ska synkroniseras med datorn](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)för mer   information.</span><span class="sxs-lookup"><span data-stu-id="6f148-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="6f148-124">Du måste slutföra detta för din personliga OneDrive och OneDrive för företag.</span><span class="sxs-lookup"><span data-stu-id="6f148-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>