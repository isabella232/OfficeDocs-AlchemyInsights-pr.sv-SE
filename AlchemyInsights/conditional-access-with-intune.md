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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505012"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="69ee5-102">Villkorad tillgång med Intune</span><span class="sxs-lookup"><span data-stu-id="69ee5-102">Conditional Access with Intune</span></span>

<span data-ttu-id="69ee5-103">**Villkorad tillgång** med Intune kräver 3 steg:</span><span class="sxs-lookup"><span data-stu-id="69ee5-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="69ee5-104">Skapa en **Princip för villkorlig åtkomst** som definierar vilka resurser skyddas och vad villkor måste uppfyllas för att få tillgång till dessa resurser.</span><span class="sxs-lookup"><span data-stu-id="69ee5-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="69ee5-105">En enhet måste till exempel vara kompatibelt innan åtkomst till företagets e-post.</span><span class="sxs-lookup"><span data-stu-id="69ee5-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="69ee5-106">Skapa en **Princip för överensstämmelse** om du vill definiera inställningar som måste vara uppfyllda innan enheten anses vara kompatibla.</span><span class="sxs-lookup"><span data-stu-id="69ee5-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="69ee5-107">En enhet måste ha en PIN-kod med minst 6 siffror innan den anses vara kompatibla.</span><span class="sxs-lookup"><span data-stu-id="69ee5-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="69ee5-108">Att säkerställa både **Efterlevnad** och **Principer för villkorlig åtkomst** är riktade till önskad grupper av användare.</span><span class="sxs-lookup"><span data-stu-id="69ee5-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="69ee5-109">Du kan behöva skapa specifika grupper av användare i Active Directory i Azure.</span><span class="sxs-lookup"><span data-stu-id="69ee5-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="69ee5-110">Läs mer:</span><span class="sxs-lookup"><span data-stu-id="69ee5-110">Read more:</span></span>
  
- [<span data-ttu-id="69ee5-111">Metodtips för villkorlig åtkomst</span><span class="sxs-lookup"><span data-stu-id="69ee5-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="69ee5-112">Komma igång med villkorad tillgång</span><span class="sxs-lookup"><span data-stu-id="69ee5-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

