---
title: Korrigera fel i 0x8004de40 i OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133994"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="e19b0-102">Korrigera fel i 0x8004de40 i OneDrive</span><span class="sxs-lookup"><span data-stu-id="e19b0-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="e19b0-103">Om du får felmeddelandet 0x8004de40 med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="e19b0-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="e19b0-104">Starta om datorn när du är ansluten till akitv Directory-domän.</span><span class="sxs-lookup"><span data-stu-id="e19b0-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="e19b0-105">Om en omstart inte löser problemet, koppla från och återansluta enheten från Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e19b0-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="e19b0-106">**Obs**: du bör vara på företagets nätverk när du utför dessa steg.</span><span class="sxs-lookup"><span data-stu-id="e19b0-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="e19b0-107">Inte utföra dessa steg när du inte kan ansluta till ditt företags infrastruktur (t.ex, under resa).</span><span class="sxs-lookup"><span data-stu-id="e19b0-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="e19b0-108">Öppna en kommandotolk.</span><span class="sxs-lookup"><span data-stu-id="e19b0-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="e19b0-109">Öppna en kommandotolk Klicka på - **Start**, högerklicka på **Kommandotolken**och klicka sedan på **Kör som administratör**.</span><span class="sxs-lookup"><span data-stu-id="e19b0-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="e19b0-110">*Dsregcmd /leave* och tryck på **RETUR**.</span><span class="sxs-lookup"><span data-stu-id="e19b0-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="e19b0-111">När du är klar, *dsregcmd, /join* och tryck på **RETUR**.</span><span class="sxs-lookup"><span data-stu-id="e19b0-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="e19b0-112">Stäng Kommandotolken när du är färdig.</span><span class="sxs-lookup"><span data-stu-id="e19b0-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="e19b0-113">Starta om datorn och logga in på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e19b0-113">Reboot the computer, and log into OneDrive.</span></span>