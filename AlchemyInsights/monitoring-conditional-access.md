---
title: Övervakning av villkorad tillgång
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538793"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="0e331-102">Övervakning av villkorlig åtkomst för Exchange</span><span class="sxs-lookup"><span data-stu-id="0e331-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="0e331-103">Riktade med villkorad tillgång användare får ett e-postmeddelanden om de inte uppfyller kraven i din organisation åtkomst.</span><span class="sxs-lookup"><span data-stu-id="0e331-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0e331-104">Lös, rekommenderar vi en eller flera av följande lösningar:</span><span class="sxs-lookup"><span data-stu-id="0e331-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="0e331-105">Om enheten antas vara anmäld, informera användaren att gå till appen företagsportal och kontrollera att det visas i företagets Portal.</span><span class="sxs-lookup"><span data-stu-id="0e331-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0e331-106">Användaren bör registrera enheten om den inte.</span><span class="sxs-lookup"><span data-stu-id="0e331-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="0e331-107">Gå till Azure portal **Intune \> överensstämmelse med enheten**.</span><span class="sxs-lookup"><span data-stu-id="0e331-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="0e331-108">Klicka på **enheten överensstämmelse**under **Bildskärm** .</span><span class="sxs-lookup"><span data-stu-id="0e331-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="0e331-109">Visa enheten överensstämmelse rapporten för att kontrollera att användarens enhet är markerad som kompatibla.</span><span class="sxs-lookup"><span data-stu-id="0e331-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="0e331-110">Gå till Azure portal **Intune \> överensstämmelse med enheten**.</span><span class="sxs-lookup"><span data-stu-id="0e331-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="0e331-111">Klicka på **principer**under **Hantera**.</span><span class="sxs-lookup"><span data-stu-id="0e331-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="0e331-112">I listan över principer för att kontrollera att en profil har tilldelats användarens enhet.</span><span class="sxs-lookup"><span data-stu-id="0e331-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0e331-113">Om ingen profil tilldelas Intune inte bekräfta överensstämmelse Enhetsstatus.</span><span class="sxs-lookup"><span data-stu-id="0e331-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="0e331-114">Redigera Användartilldelning villkorad tillgång.</span><span class="sxs-lookup"><span data-stu-id="0e331-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="0e331-115">Gå till Azure portal **Intune \> villkorad tillgång \> principer**</span><span class="sxs-lookup"><span data-stu-id="0e331-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="0e331-116">Välj en princip i listan</span><span class="sxs-lookup"><span data-stu-id="0e331-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="0e331-117">Klicka på **användare och grupper**</span><span class="sxs-lookup"><span data-stu-id="0e331-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="0e331-118">Om du vill ange en viss policy på någon att lägga till dem till **listan** .</span><span class="sxs-lookup"><span data-stu-id="0e331-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="0e331-119">Om du vill säkerställa att en person utelämnas från principen att lägga till dem i listan **Exkludera** .</span><span class="sxs-lookup"><span data-stu-id="0e331-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="0e331-120">Läs mer: [hur du övervaka villkorad tillgång enheter](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="0e331-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

