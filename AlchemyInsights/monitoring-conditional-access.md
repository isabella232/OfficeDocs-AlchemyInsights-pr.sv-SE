---
title: Övervaka villkorlig åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702921"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="e568c-102">Övervaka villkorlig åtkomst för Exchange</span><span class="sxs-lookup"><span data-stu-id="e568c-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="e568c-103">Användare riktade mot villkorsstyrd åtkomst får ett e-postmeddelande om de inte uppfyller åtkomst kraven för organisationen.</span><span class="sxs-lookup"><span data-stu-id="e568c-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e568c-104">För att lösa problemet rekommenderar vi en eller flera av följande lösningar:</span><span class="sxs-lookup"><span data-stu-id="e568c-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="e568c-105">Om enheten är registrerad kan du uppmana användaren att gå till företagsportalsappen och kontrol lera att den visas i företags portalen.</span><span class="sxs-lookup"><span data-stu-id="e568c-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e568c-106">Om det inte gör det bör användaren registrera enheten.</span><span class="sxs-lookup"><span data-stu-id="e568c-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="e568c-107">I Azure-portalen går du till **Intune- \> enhetsupptäckning**.</span><span class="sxs-lookup"><span data-stu-id="e568c-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e568c-108">Klicka på **enhets överensstämmelse**under **bildskärm** .</span><span class="sxs-lookup"><span data-stu-id="e568c-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="e568c-109">Visa din enhets kompatibilitetsstatus för att kontrol lera att användarens enhet är markerad som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="e568c-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="e568c-110">I Azure-portalen går du till **Intune- \> enhetsupptäckning**.</span><span class="sxs-lookup"><span data-stu-id="e568c-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e568c-111">Under **Hantera**klickar du på **principer**.</span><span class="sxs-lookup"><span data-stu-id="e568c-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="e568c-112">I listan över efterlevnadsprinciper kontrollerar du att en profil har tilldelats till din användares enhet.</span><span class="sxs-lookup"><span data-stu-id="e568c-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e568c-113">Om ingen profil är tilldelad kan Intune inte bekräfta status för enhetens efterlevnad.</span><span class="sxs-lookup"><span data-stu-id="e568c-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="e568c-114">Redigera användarens villkorliga åtkomst tilldelning.</span><span class="sxs-lookup"><span data-stu-id="e568c-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="e568c-115">I Azure-portalen går du till **Intune \> \> policy för villkorsstyrd åtkomst**</span><span class="sxs-lookup"><span data-stu-id="e568c-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="e568c-116">Välj en princip i listan</span><span class="sxs-lookup"><span data-stu-id="e568c-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="e568c-117">Klicka på **användare och grupper**</span><span class="sxs-lookup"><span data-stu-id="e568c-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="e568c-118">Om du vill rikta en viss princip till någon kan du lägga till dem i listan **ta med** .</span><span class="sxs-lookup"><span data-stu-id="e568c-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="e568c-119">Om du vill se till att en person utelämnas från policyn lägger du till den i listan **undantag** .</span><span class="sxs-lookup"><span data-stu-id="e568c-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="e568c-120">Läs mer: [så här övervakar du enheter för villkorsstyrd åtkomst](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="e568c-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

