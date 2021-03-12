---
title: Använda villkorsstyrd åtkomst med Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749264"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="0153c-102">Använda villkorsstyrd åtkomst med Intune</span><span class="sxs-lookup"><span data-stu-id="0153c-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="0153c-103">Användning av villkorsstyrd åtkomst med Intune kräver 3 steg:</span><span class="sxs-lookup"><span data-stu-id="0153c-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="0153c-104">Skapa en efterlevnadsprincip för att definiera inställningar som måste uppfyllas för att enheten ska anses vara kompatibel. En enhet måste ha en PIN-kod med minst 6 siffror innan den anses vara kompatibel.</span><span class="sxs-lookup"><span data-stu-id="0153c-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="0153c-105">Skapa en princip för villkorsstyrd åtkomst som definierar vilka resurser som ska skyddas och vilka villkor som måste uppfyllas för att komma åt dessa resurser. En enhet måste till exempel vara kompatibel innan åtkomst ges till företagets e-post.</span><span class="sxs-lookup"><span data-stu-id="0153c-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="0153c-106">Se till att både efterlevnadsprinciper och villkorsstyrda åtkomstprinciper är riktade till önskade grupper av användare. Det kan kräva att du skapar specifika grupper av användare i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0153c-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="0153c-107">Läs mer...</span><span class="sxs-lookup"><span data-stu-id="0153c-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
