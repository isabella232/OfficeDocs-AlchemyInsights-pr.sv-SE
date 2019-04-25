---
title: Villkorad tillgång med Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393559"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="b1ca0-102">Villkorad tillgång med Intune</span><span class="sxs-lookup"><span data-stu-id="b1ca0-102">Conditional Access with Intune</span></span>

<span data-ttu-id="b1ca0-103">**Villkorad tillgång** med Intune kräver 3 steg:</span><span class="sxs-lookup"><span data-stu-id="b1ca0-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="b1ca0-104">Skapa en **Princip för villkorlig åtkomst** som definierar vilka resurser skyddas och vad villkor måste uppfyllas för att få tillgång till dessa resurser.</span><span class="sxs-lookup"><span data-stu-id="b1ca0-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="b1ca0-105">En enhet måste till exempel vara kompatibelt innan åtkomst till företagets e-post.</span><span class="sxs-lookup"><span data-stu-id="b1ca0-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="b1ca0-106">Skapa en **Princip för överensstämmelse** om du vill definiera inställningar som måste vara uppfyllda innan enheten anses vara kompatibla.</span><span class="sxs-lookup"><span data-stu-id="b1ca0-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="b1ca0-107">En enhet måste ha en PIN-kod med minst 6 siffror innan den anses vara kompatibla.</span><span class="sxs-lookup"><span data-stu-id="b1ca0-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="b1ca0-108">Att säkerställa både **Efterlevnad** och **Principer för villkorlig åtkomst** är riktade till önskad grupper av användare.</span><span class="sxs-lookup"><span data-stu-id="b1ca0-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="b1ca0-109">Du kan behöva skapa specifika grupper av användare i Active Directory i Azure.</span><span class="sxs-lookup"><span data-stu-id="b1ca0-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="b1ca0-110">Läs mer:</span><span class="sxs-lookup"><span data-stu-id="b1ca0-110">Read more:</span></span>
  
- [<span data-ttu-id="b1ca0-111">Metodtips för villkorlig åtkomst</span><span class="sxs-lookup"><span data-stu-id="b1ca0-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="b1ca0-112">Komma igång med villkorad tillgång</span><span class="sxs-lookup"><span data-stu-id="b1ca0-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

