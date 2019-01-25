---
title: Övervakning av villkorad tillgång
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29491835"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="c7ffe-102">Övervakning av villkorad tillgång</span><span class="sxs-lookup"><span data-stu-id="c7ffe-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="c7ffe-p101">Riktade med villkorad tillgång användare får ett e-postmeddelanden om de inte uppfyller kraven i din organisation åtkomst. Lös, rekommenderar vi en eller flera av följande lösningar:</span><span class="sxs-lookup"><span data-stu-id="c7ffe-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="c7ffe-p102">Om enheten antas vara anmäld, informera användaren att gå till appen företagsportal och kontrollera att det visas i företagets Portal. Användaren bör registrera enheten om den inte.</span><span class="sxs-lookup"><span data-stu-id="c7ffe-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="c7ffe-p103">Gå till Azure portal **Intune \> överensstämmelse med enheten**. Klicka på **enheten överensstämmelse**under **Bildskärm** . Visa enheten överensstämmelse rapporten för att kontrollera att användarens enhet är markerad som kompatibla.</span><span class="sxs-lookup"><span data-stu-id="c7ffe-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="c7ffe-p104">Gå till Azure portal **Intune \> överensstämmelse med enheten**. Klicka på **principer**under **Hantera**. I listan över principer för att kontrollera att en profil har tilldelats användarens enhet. Om ingen profil tilldelas Intune inte bekräfta överensstämmelse Enhetsstatus.</span><span class="sxs-lookup"><span data-stu-id="c7ffe-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="c7ffe-114">Redigera Användartilldelning villkorad tillgång.</span><span class="sxs-lookup"><span data-stu-id="c7ffe-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="c7ffe-115">Gå till Azure portal **Intune \> villkorad tillgång \> principer**</span><span class="sxs-lookup"><span data-stu-id="c7ffe-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="c7ffe-116">Välj en princip i listan</span><span class="sxs-lookup"><span data-stu-id="c7ffe-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="c7ffe-117">Klicka på **användare och grupper**</span><span class="sxs-lookup"><span data-stu-id="c7ffe-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="c7ffe-p105">Om du vill ange en viss policy på någon att lägga till dem till **listan** . Om du vill säkerställa att en person utelämnas från principen att lägga till dem i listan **Exkludera** .</span><span class="sxs-lookup"><span data-stu-id="c7ffe-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="c7ffe-120">Läs mer: [hur du övervaka villkorad tillgång enheter](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="c7ffe-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

