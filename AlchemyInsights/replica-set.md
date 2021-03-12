---
title: Replikuppsättning
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714585"
---
# <a name="replica-set"></a><span data-ttu-id="00845-102">Replikuppsättning</span><span class="sxs-lookup"><span data-stu-id="00845-102">Replica set</span></span>

<span data-ttu-id="00845-103">AADDS kallas även för den hanterade domänen.</span><span class="sxs-lookup"><span data-stu-id="00845-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="00845-104">Det är faktiskt två domänkontrollanter som körs och underhålls av backend.</span><span class="sxs-lookup"><span data-stu-id="00845-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="00845-105">De två dc-erna innehåller ett huvud-DC och en replikerings-DC.</span><span class="sxs-lookup"><span data-stu-id="00845-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="00845-106">Säkerhetskopior i AADDS (hanterad domän) är en automatiserad process som hanteras av Azure-plattformen.</span><span class="sxs-lookup"><span data-stu-id="00845-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="00845-107">I händelse av ett problem med din hanterade domän kan Azure-supporten hjälpa dig att återställa från säkerhetskopiering.</span><span class="sxs-lookup"><span data-stu-id="00845-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="00845-108">Du skapar varje uppsättning av repliker i ett virtuellt nätverk.</span><span class="sxs-lookup"><span data-stu-id="00845-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="00845-109">Varje virtuellt nätverk måste peered to every other virtual network that hosts a managed domain's replica set.</span><span class="sxs-lookup"><span data-stu-id="00845-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="00845-110">Den här konfigurationen skapar en nättopologi som stöder katalogreplikering.</span><span class="sxs-lookup"><span data-stu-id="00845-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="00845-111">Ett virtuellt nätverk kan ha stöd för flera replikuppsättningar, förutsatt att varje uppsättning av repliker finns i ett annat virtuellt undernät.</span><span class="sxs-lookup"><span data-stu-id="00845-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="00845-112">Mer information om replikuppsättningar finns i Concepts [Replica-uppsättningar.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="00845-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
