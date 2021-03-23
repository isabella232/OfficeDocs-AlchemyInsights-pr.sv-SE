---
title: Om Yammer-administratörer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038126"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="4abea-102">Om Yammer-administratörer</span><span class="sxs-lookup"><span data-stu-id="4abea-102">About Yammer admins</span></span>

<span data-ttu-id="4abea-103">**Nätverksadministratörer**</span><span class="sxs-lookup"><span data-stu-id="4abea-103">**Network admins**</span></span>

<span data-ttu-id="4abea-104">Globala administratörer framhävs automatiskt till rollen verifierad administratör i ett Yammer-nätverk.</span><span class="sxs-lookup"><span data-stu-id="4abea-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="4abea-105">I följande fall kan den här kampanjen inte ske på rätt sätt:</span><span class="sxs-lookup"><span data-stu-id="4abea-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="4abea-106">Det finns flera Yammer-nätverk och administratören loggas in på fel nätverk.</span><span class="sxs-lookup"><span data-stu-id="4abea-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="4abea-107">[Nätverkskonsolidering](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) krävs för att komma till ett Yammer-nätverk.</span><span class="sxs-lookup"><span data-stu-id="4abea-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="4abea-108">Azure PIM används.</span><span class="sxs-lookup"><span data-stu-id="4abea-108">Azure PIM is being used.</span></span> <span data-ttu-id="4abea-109">Användaren kanske inte är global administratör tillräckligt länge för att kampanjen ska kunna ske.</span><span class="sxs-lookup"><span data-stu-id="4abea-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="4abea-110">En kommande uppdatering av Yammer kan lösa problemet, men det är bäst att göra användarna till globala administratörer manuellt.</span><span class="sxs-lookup"><span data-stu-id="4abea-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="4abea-111">Det finns ett synkroniseringsproblem med Yammer-nätverket.</span><span class="sxs-lookup"><span data-stu-id="4abea-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="4abea-112">I det här fallet krävs en supportbegäran för ytterligare undersökning.</span><span class="sxs-lookup"><span data-stu-id="4abea-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="4abea-113">Mer information om administratörsroller i Yammer finns [i Hantera Yammer-administratörer.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)</span><span class="sxs-lookup"><span data-stu-id="4abea-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="4abea-114">**Gruppadministratörer**</span><span class="sxs-lookup"><span data-stu-id="4abea-114">**Group admins**</span></span>

<span data-ttu-id="4abea-115">Gruppadministratörer för Microsoft 365-anslutna grupper synkroniseras med gruppmedlemskap från Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4abea-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="4abea-116">För stora grupper kan synkroniseringen ta en längre tid.</span><span class="sxs-lookup"><span data-stu-id="4abea-116">For large groups, this sync can take an extended period.</span></span>
