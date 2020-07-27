---
title: Princip för programskydd
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423959"
---
# <a name="application-protection-policy"></a><span data-ttu-id="d579d-102">Princip för programskydd</span><span class="sxs-lookup"><span data-stu-id="d579d-102">Application protection policy</span></span>

<span data-ttu-id="d579d-103">Om du inte har en ny till Application Protection Policy (APP) kan du läsa [översikten över appskyddsprinciper](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="d579d-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="d579d-104">Lär dig hur du [skapar och tilldelar principer för appskydd](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="d579d-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="d579d-105">Krav på programskydd:</span><span class="sxs-lookup"><span data-stu-id="d579d-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="d579d-106">Användaren har en Intune- eller EMS-licens.</span><span class="sxs-lookup"><span data-stu-id="d579d-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="d579d-107">Användaren tillhör en grupp som omfattas av programskyddsprinciper.</span><span class="sxs-lookup"><span data-stu-id="d579d-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="d579d-108">Endast en företagsanvändare är inloggad i skyddade appar på en enhet.</span><span class="sxs-lookup"><span data-stu-id="d579d-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="d579d-109">Programmet har [implementerat Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="d579d-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="d579d-110">En lista över appar som stöder SDK finns [i Microsoft Intune-skyddade appar](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="d579d-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="d579d-111">Principer gäller när en användare som uppfyller ovanstående krav loggar in på en Intune SDK-aktiverad app.</span><span class="sxs-lookup"><span data-stu-id="d579d-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="d579d-112">Det enklaste sättet att avgöra om en princip tillämpas är genom att kräva att användaren anger en pin i principen.</span><span class="sxs-lookup"><span data-stu-id="d579d-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="d579d-113">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="d579d-113">For more information, see:</span></span>

[<span data-ttu-id="d579d-114">Vanliga frågor och svar om APP/MAM-felsökning</span><span class="sxs-lookup"><span data-stu-id="d579d-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="d579d-115">Så här validerar du principinställningarna för appskydd</span><span class="sxs-lookup"><span data-stu-id="d579d-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="d579d-116">Förstå leveranstid för appskyddsprincip</span><span class="sxs-lookup"><span data-stu-id="d579d-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="d579d-117">Så här övervakar du appskyddsprinciper</span><span class="sxs-lookup"><span data-stu-id="d579d-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)