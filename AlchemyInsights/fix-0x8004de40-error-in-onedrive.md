---
title: Åtgärda 0x8004de40-fel i OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755866"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="8ed2d-102">Åtgärda 0x8004de40-fel i OneDrive</span><span class="sxs-lookup"><span data-stu-id="8ed2d-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="8ed2d-103">Om du får ett 0x8004de40-fel med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="8ed2d-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="8ed2d-104">Starta om den aktuella datorn när du är ansluten till din Acitve Directory-domän.</span><span class="sxs-lookup"><span data-stu-id="8ed2d-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="8ed2d-105">Om en omstart inte löser problemet, ta bort kopplingen och Anslut din enhet från Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8ed2d-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="8ed2d-106">**Du bör**vara i företagsnätverket när du utför dessa steg.</span><span class="sxs-lookup"><span data-stu-id="8ed2d-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="8ed2d-107">Utför inte de här stegen när du inte kan ansluta till företagets infrastruktur (till exempel när du reser).</span><span class="sxs-lookup"><span data-stu-id="8ed2d-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="8ed2d-108">Öppna en upphöjd kommandotolk.</span><span class="sxs-lookup"><span data-stu-id="8ed2d-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="8ed2d-109">Om du vill öppna en upphöjd kommandotolk klickar du på **Start**, högerklickar på **Kommandotolken**och klickar sedan på **Kör som administratör**.</span><span class="sxs-lookup"><span data-stu-id="8ed2d-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="8ed2d-110">Skriv *dsregcmd/Leave* och tryck på **RETUR**.</span><span class="sxs-lookup"><span data-stu-id="8ed2d-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="8ed2d-111">När du är klar skriver du *dsregcmd/Join* och trycker på **RETUR**.</span><span class="sxs-lookup"><span data-stu-id="8ed2d-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="8ed2d-112">Stäng Kommandotolken när du är klar.</span><span class="sxs-lookup"><span data-stu-id="8ed2d-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="8ed2d-113">Starta om datorn och logga in på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8ed2d-113">Reboot the computer, and log into OneDrive.</span></span>