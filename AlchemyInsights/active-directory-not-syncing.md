---
title: Active Directory synkroniseras inte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265274"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="852c1-102">Active Directory synkroniseras inte</span><span class="sxs-lookup"><span data-stu-id="852c1-102">Active Directory not syncing</span></span>

<span data-ttu-id="852c1-103">Om du får synkroniseringsfel, till exempel "ingen ny synkronisering" eller märker katalogsynkroniseringsstatus en office-administratörsportal säger: "Senast synkroniserad mer än 3 dagar sedan", kan det hända att AADConnect har felaktiga inställningar eller otillräckliga behörigheter för att utföra en synkronisering.</span><span class="sxs-lookup"><span data-stu-id="852c1-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="852c1-104">Om du installerar om AADConnect med hjälp av expressinställningar kan problemet lösas snabbt:</span><span class="sxs-lookup"><span data-stu-id="852c1-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="852c1-105">[Ladda ner den senaste versionen av AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="852c1-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="852c1-106">[Följ instruktionerna för expressinstallation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="852c1-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="852c1-107">Mer information om AADConnect-tjänstkonton finns i [Azure AD Connect: Konton och behörigheter](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="852c1-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
