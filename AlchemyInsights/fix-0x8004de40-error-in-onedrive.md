---
title: Åtgärda 0x8004de40-fel i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716046"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="5d932-102">Åtgärda 0x8004de40-fel i OneDrive</span><span class="sxs-lookup"><span data-stu-id="5d932-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="5d932-103">Om du får ett 0x8004de40-fel med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="5d932-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="5d932-104">Starta om den dator som påverkas när den är ansluten till Acitve Directory-domänen.</span><span class="sxs-lookup"><span data-stu-id="5d932-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="5d932-105">Om en omstart inte löser problemet kan du koppla bort och ansluta till enheten från Azure AD igen.</span><span class="sxs-lookup"><span data-stu-id="5d932-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="5d932-106">**Du**bör vara i företagets nätverk när du utför dessa steg.</span><span class="sxs-lookup"><span data-stu-id="5d932-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="5d932-107">Utför inte de här stegen när du inte kan ansluta till företagets infrastruktur (till exempel när du reser).</span><span class="sxs-lookup"><span data-stu-id="5d932-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="5d932-108">Öppna en upphöjd kommandotolk.</span><span class="sxs-lookup"><span data-stu-id="5d932-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="5d932-109">Om du vill öppna en upphöjd kommandotolk klickar du på - **Starta**, högerklickar på **Kommandotolken**och klickar sedan på **Kör som administratör**.</span><span class="sxs-lookup"><span data-stu-id="5d932-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="5d932-110">Skriv *dsregcmd /leave* och tryck på **Retur**.</span><span class="sxs-lookup"><span data-stu-id="5d932-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="5d932-111">När du är klar skriver du *dsregcmd /join* och trycker på **Retur**.</span><span class="sxs-lookup"><span data-stu-id="5d932-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="5d932-112">När du är klar stänger du kommandotolken.</span><span class="sxs-lookup"><span data-stu-id="5d932-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="5d932-113">Starta om datorn och logga in på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5d932-113">Reboot the computer, and log into OneDrive.</span></span>