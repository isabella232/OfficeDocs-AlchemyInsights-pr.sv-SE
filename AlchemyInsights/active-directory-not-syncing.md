---
title: Active Directory synkroniseras inte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822869"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="6a414-102">Active Directory synkroniseras inte</span><span class="sxs-lookup"><span data-stu-id="6a414-102">Active Directory not syncing</span></span>

<span data-ttu-id="6a414-103">Om du får synkroniseringsfel, till exempel "ingen ny synkronisering", eller om katalogsynkroniseringsstatusen visas i Office-administratörsportalen "Synkroniserades senast för mer än 3 dagar sedan" kan det vara så att AADConnect har felaktiga inställningar eller otillräckliga behörigheter för att utföra en synkronisering.</span><span class="sxs-lookup"><span data-stu-id="6a414-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="6a414-104">Om du installerar om AADConnect med hjälp av standardinställningarna kan problemet snabbt lösas:</span><span class="sxs-lookup"><span data-stu-id="6a414-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="6a414-105">[Ladda ned den senaste versionen av AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="6a414-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="6a414-106">[Följ anvisningarna för expressinstallation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="6a414-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="6a414-107">Mer information om AADConnect-tjänstkonton finns i [Azure AD Connect: Konton och behörigheter.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="6a414-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
