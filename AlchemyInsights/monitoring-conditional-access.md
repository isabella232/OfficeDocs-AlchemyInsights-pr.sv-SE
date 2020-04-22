---
title: Övervaka villkorlig åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713736"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="41a01-102">Övervaka villkorlig åtkomst för Exchange</span><span class="sxs-lookup"><span data-stu-id="41a01-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="41a01-103">Användare som är inriktade på villkorlig åtkomst får ett e-postmeddelande om de inte uppfyller organisationens åtkomstkrav.</span><span class="sxs-lookup"><span data-stu-id="41a01-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="41a01-104">För att lösa det rekommenderar vi en eller flera av följande lösningar:</span><span class="sxs-lookup"><span data-stu-id="41a01-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="41a01-105">Om enheten antas vara registrerad, råda användaren att gå till företagsportalappen och kontrollera att den visas i företagsportalen.</span><span class="sxs-lookup"><span data-stu-id="41a01-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="41a01-106">Om den inte gör det bör användaren registrera enheten.</span><span class="sxs-lookup"><span data-stu-id="41a01-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="41a01-107">Gå till **Intune \> Device compliance**i Azure-portalen .</span><span class="sxs-lookup"><span data-stu-id="41a01-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="41a01-108">Klicka på **Enhetsefterlevnad**under **Bildskärm.**</span><span class="sxs-lookup"><span data-stu-id="41a01-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="41a01-109">Visa enhetens efterlevnadsrapport för att kontrollera att användarens enhet är markerad som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="41a01-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="41a01-110">Gå till **Intune \> Device compliance**i Azure-portalen .</span><span class="sxs-lookup"><span data-stu-id="41a01-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="41a01-111">Klicka på **Principer**under **Hantera.**</span><span class="sxs-lookup"><span data-stu-id="41a01-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="41a01-112">Kontrollera att en profil har tilldelats användarens enhet i listan över efterlevnadsprinciper.</span><span class="sxs-lookup"><span data-stu-id="41a01-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="41a01-113">Om ingen profil har tilldelats kan Intune inte bekräfta enhetens efterlevnadsstatus.</span><span class="sxs-lookup"><span data-stu-id="41a01-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="41a01-114">Redigera användarens tilldelning av villkorlig åtkomst.</span><span class="sxs-lookup"><span data-stu-id="41a01-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="41a01-115">Gå till **Intune-principer \> för \> villkorlig åtkomst i** Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="41a01-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="41a01-116">Välj en princip i listan</span><span class="sxs-lookup"><span data-stu-id="41a01-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="41a01-117">Klicka på **Användare och grupper**</span><span class="sxs-lookup"><span data-stu-id="41a01-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="41a01-118">Om du vill rikta en viss princip mot någon lägger du till dem i listan **Inkludera.**</span><span class="sxs-lookup"><span data-stu-id="41a01-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="41a01-119">Om du vill vara säkra på att en person utelämnas från principen lägger du till dem i listan **Uteslut.**</span><span class="sxs-lookup"><span data-stu-id="41a01-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="41a01-120">Läs mer: [Så här övervakar du enheter med villkorlig åtkomst](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="41a01-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

