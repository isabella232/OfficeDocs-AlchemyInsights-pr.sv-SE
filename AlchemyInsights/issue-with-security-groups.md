---
title: Problem med säkerhetsgrupper
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177634"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="65d90-102">Problem med säkerhetsgrupper</span><span class="sxs-lookup"><span data-stu-id="65d90-102">Issue with security groups</span></span>

<span data-ttu-id="65d90-103">**Om du får nätverksfel AADDS104**</span><span class="sxs-lookup"><span data-stu-id="65d90-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="65d90-104">Ogiltiga nätverkssäkerhetsgruppsregler är den vanligaste orsaken till nätverksfel för Azure Active Directory DS (AD DS).</span><span class="sxs-lookup"><span data-stu-id="65d90-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="65d90-105">Nätverkssäkerhetsgruppen för det virtuella nätverket måste tillåta åtkomst till specifika portar och protokoll.</span><span class="sxs-lookup"><span data-stu-id="65d90-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="65d90-106">Om dessa portar är blockerade kan Azure-plattformen inte övervaka eller uppdatera den hanterade domänen.</span><span class="sxs-lookup"><span data-stu-id="65d90-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="65d90-107">Synkroniseringen mellan Azure AD och Azure AD DS påverkas också.</span><span class="sxs-lookup"><span data-stu-id="65d90-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="65d90-108">Se till att ha standardportarna öppna för att undvika avbrott i tjänsten.</span><span class="sxs-lookup"><span data-stu-id="65d90-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="65d90-109">Information om hur du förstår och löser vanliga varningar för konfigurationsproblem för säkerhetsgrupper i nätverket finns i [Lägga till och verifiera säkerhetsgrupper.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)</span><span class="sxs-lookup"><span data-stu-id="65d90-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
