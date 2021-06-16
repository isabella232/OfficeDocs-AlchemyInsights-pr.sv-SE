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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930993"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="7b18f-102">Active Directory synkroniseras inte</span><span class="sxs-lookup"><span data-stu-id="7b18f-102">Active Directory not syncing</span></span>

<span data-ttu-id="7b18f-103">Om du får synkroniseringsfel, till exempel "ingen ny synkronisering", eller om katalogsynkroniseringsstatusen visas i administrationsportalen för Office står det "Senaste synkroniseringen för mer än 3 dagar sedan" kan det vara så att AADConnect har felaktiga inställningar eller otillräckliga behörigheter för att utföra en synkronisering.</span><span class="sxs-lookup"><span data-stu-id="7b18f-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="7b18f-104">Om du installerar om AADConnect med standardinställningarna kan problemet snabbt lösas:</span><span class="sxs-lookup"><span data-stu-id="7b18f-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="7b18f-105">[Ladda ned den senaste versionen av AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="7b18f-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="7b18f-106">[Följ anvisningarna för expressinstallation](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="7b18f-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="7b18f-107">Azure AD Connect måste installeras på Windows Server 2012 eller senare.</span><span class="sxs-lookup"><span data-stu-id="7b18f-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="7b18f-108">Servern måste vara domänansluten och kan vara en domänkontrollant eller en medlemsserver.</span><span class="sxs-lookup"><span data-stu-id="7b18f-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="7b18f-109">En fullständig lista över krav och förutsättningar Anslut Azure AD finns i Förutsättningar [för Azure AD Anslut.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="7b18f-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="7b18f-110">Mer information om AADConnect-tjänstkonton finns i [Azure AD Anslut: Konton och behörigheter.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="7b18f-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
