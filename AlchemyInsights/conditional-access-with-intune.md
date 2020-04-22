---
title: Villkorlig åtkomst med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706039"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="6fe82-102">Villkorlig åtkomst med Intune</span><span class="sxs-lookup"><span data-stu-id="6fe82-102">Conditional Access with Intune</span></span>

<span data-ttu-id="6fe82-103">Om du använder **villkorlig åtkomst** med Intune krävs 3 steg:</span><span class="sxs-lookup"><span data-stu-id="6fe82-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="6fe82-104">Skapa en **princip för villkorlig åtkomst** som definierar vilka resurser som skyddas och vilka villkor som måste uppfyllas för att komma åt dessa resurser.</span><span class="sxs-lookup"><span data-stu-id="6fe82-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="6fe82-105">En enhet måste till exempel vara kompatibel innan den får åtkomst till företagets e-post.</span><span class="sxs-lookup"><span data-stu-id="6fe82-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="6fe82-106">Skapa en **efterlevnadsprincip** för att definiera inställningar som måste uppfyllas innan enheten anses vara kompatibel.</span><span class="sxs-lookup"><span data-stu-id="6fe82-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="6fe82-107">En enhet måste till exempel ha en stift på minst 6 siffror innan den anses vara kompatibel.</span><span class="sxs-lookup"><span data-stu-id="6fe82-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="6fe82-108">Se till att både **efterlevnadsprinciper** och **principer för villkorlig åtkomst** är inriktade på önskade användargrupper.</span><span class="sxs-lookup"><span data-stu-id="6fe82-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="6fe82-109">Detta kan kräva att du skapar specifika grupper av användare i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6fe82-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="6fe82-110">Läs mer:</span><span class="sxs-lookup"><span data-stu-id="6fe82-110">Read more:</span></span>
  
- [<span data-ttu-id="6fe82-111">Metodtips för villkorlig åtkomst</span><span class="sxs-lookup"><span data-stu-id="6fe82-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="6fe82-112">Komma igång med villkorlig åtkomst</span><span class="sxs-lookup"><span data-stu-id="6fe82-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

