---
title: Åtgärda 0x8004de40-fel i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745148"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="ef115-102">Åtgärda 0x8004de40-fel i OneDrive</span><span class="sxs-lookup"><span data-stu-id="ef115-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="ef115-103">Om du får ett 0x8004de40-fel med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="ef115-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="ef115-104">Starta om datorn när den är ansluten till din Acitve-katalog.</span><span class="sxs-lookup"><span data-stu-id="ef115-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="ef115-105">Om det inte går att åtgärda problemet kan du koppla från och återansluta till enheten från Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ef115-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="ef115-106">**Obs!** du bör vara på företagets nätverk när du utför de här stegen.</span><span class="sxs-lookup"><span data-stu-id="ef115-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="ef115-107">Utför inte de här stegen när du inte kan ansluta till företagets infrastruktur (till exempel när du reser).</span><span class="sxs-lookup"><span data-stu-id="ef115-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="ef115-108">Öppna en upphöjd kommando tolk.</span><span class="sxs-lookup"><span data-stu-id="ef115-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="ef115-109">Öppna en upphöjd kommando tolk genom att klicka på **Start**, högerklicka på **kommando tolken**och klicka sedan på **Kör som administratör**.</span><span class="sxs-lookup"><span data-stu-id="ef115-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="ef115-110">Skriv *dsregcmd/Leave* och tryck på **RETUR**.</span><span class="sxs-lookup"><span data-stu-id="ef115-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="ef115-111">När du är klar skriver du *dsregcmd/Join* och trycker på **RETUR**.</span><span class="sxs-lookup"><span data-stu-id="ef115-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="ef115-112">När du är klar stänger du kommando tolken.</span><span class="sxs-lookup"><span data-stu-id="ef115-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="ef115-113">Starta om datorn och logga in på OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ef115-113">Reboot the computer, and log into OneDrive.</span></span>