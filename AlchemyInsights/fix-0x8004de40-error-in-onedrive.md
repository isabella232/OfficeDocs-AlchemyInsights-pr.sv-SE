---
title: Åtgärda 0x8004de40-fel i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052055"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="d9586-102">Åtgärda 0x8004de40-fel i OneDrive</span><span class="sxs-lookup"><span data-stu-id="d9586-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="d9586-103">Om du får ett 0x8004de40-fel med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="d9586-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="d9586-104">Starta om den aktuella datorn när du är ansluten till din Acitve Directory-domän.</span><span class="sxs-lookup"><span data-stu-id="d9586-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="d9586-105">Om en omstart inte löser problemet, ta bort kopplingen och Anslut din enhet från Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d9586-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="d9586-106">**Du bör**vara i företagsnätverket när du utför dessa steg.</span><span class="sxs-lookup"><span data-stu-id="d9586-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="d9586-107">Utför inte de här stegen när du inte kan ansluta till företagets infrastruktur (till exempel när du reser).</span><span class="sxs-lookup"><span data-stu-id="d9586-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="d9586-108">Öppna en upphöjd kommandotolk.</span><span class="sxs-lookup"><span data-stu-id="d9586-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="d9586-109">Om du vill öppna en upphöjd kommandotolk klickar du på **Start**, högerklickar på **Kommandotolken**och klickar sedan på **Kör som administratör**.</span><span class="sxs-lookup"><span data-stu-id="d9586-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="d9586-110">Skriv *dsregcmd/Leave* och tryck på **RETUR**.</span><span class="sxs-lookup"><span data-stu-id="d9586-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="d9586-111">När du är klar skriver du *dsregcmd/Join* och trycker på **RETUR**.</span><span class="sxs-lookup"><span data-stu-id="d9586-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="d9586-112">Stäng Kommandotolken när du är klar.</span><span class="sxs-lookup"><span data-stu-id="d9586-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="d9586-113">Starta om datorn och logga in på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d9586-113">Reboot the computer, and log into OneDrive.</span></span>