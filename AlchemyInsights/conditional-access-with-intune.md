---
title: Villkorad tillgång med Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492662"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="f28f4-102">Villkorad tillgång med Intune</span><span class="sxs-lookup"><span data-stu-id="f28f4-102">Conditional Access with Intune</span></span>

<span data-ttu-id="f28f4-103">**Villkorad tillgång** med Intune kräver 3 steg:</span><span class="sxs-lookup"><span data-stu-id="f28f4-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="f28f4-p101">Skapa en **Princip för villkorlig åtkomst** som definierar vilka resurser skyddas och vad villkor måste uppfyllas för att få tillgång till dessa resurser. En enhet måste till exempel vara kompatibelt innan åtkomst till företagets e-post.</span><span class="sxs-lookup"><span data-stu-id="f28f4-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="f28f4-p102">Skapa en **Princip för överensstämmelse** om du vill definiera inställningar som måste vara uppfyllda innan enheten anses vara kompatibla. En enhet måste ha en PIN-kod med minst 6 siffror innan den anses vara kompatibla.</span><span class="sxs-lookup"><span data-stu-id="f28f4-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="f28f4-p103">Att säkerställa både **Efterlevnad** och **Principer för villkorlig åtkomst** är riktade till önskad grupper av användare. Du kan behöva skapa specifika grupper av användare i Active Directory i Azure.</span><span class="sxs-lookup"><span data-stu-id="f28f4-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="f28f4-110">Läs mer</span><span class="sxs-lookup"><span data-stu-id="f28f4-110">Read more:</span></span>
  
- [<span data-ttu-id="f28f4-111">Metodtips för villkorlig åtkomst</span><span class="sxs-lookup"><span data-stu-id="f28f4-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="f28f4-112">Komma igång med villkorad tillgång</span><span class="sxs-lookup"><span data-stu-id="f28f4-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

