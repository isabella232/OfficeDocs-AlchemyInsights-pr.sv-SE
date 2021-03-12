---
title: Övervaka villkorsstyrd åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708692"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="fb7c3-102">Övervaka villkorsstyrd åtkomst för Exchange</span><span class="sxs-lookup"><span data-stu-id="fb7c3-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="fb7c3-103">Användare med villkorsstyrd åtkomst får ett e-postmeddelande om de inte uppfyller organisationens åtkomstkrav.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="fb7c3-104">Som lösning på det rekommenderar vi en eller flera av följande lösningar:</span><span class="sxs-lookup"><span data-stu-id="fb7c3-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="fb7c3-105">Om enheten antas vara registrerad kan du be användaren gå till företagsportalappen och kontrollera att den visas i företagsportalen.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="fb7c3-106">Om den inte gör det bör användaren registrera enheten.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="fb7c3-107">I Azure-portalen går du till Intune > Enhetsefterlevnad.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="fb7c3-108">Klicka på Enhetsefterlevnad under Övervaka.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="fb7c3-109">Visa rapporten över enhetsefterlevnad för att verifiera att användarens enhet är markerad som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="fb7c3-110">I Azure-portalen går du till Intune > Enhetsefterlevnad.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="fb7c3-111">Klicka på Principer under Hantera.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-111">Under Manage, click Policies.</span></span> <span data-ttu-id="fb7c3-112">Kontrollera att en profil är tilldelad till användarens enhet i listan över efterlevnadsprinciper.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="fb7c3-113">Om ingen profil har tilldelats kan Intune inte bekräfta enhetens efterlevnadsstatus.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="fb7c3-114">Redigera användarens tilldelning av villkorsstyrd åtkomst.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="fb7c3-115">Gå till Villkorsstyrda **åtkomstprinciper för Intune** i Azure  >  **Portal.**  >  </span><span class="sxs-lookup"><span data-stu-id="fb7c3-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="fb7c3-116">Välj en princip i listan.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="fb7c3-117">Klicka på Användare och grupper.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-117">Click Users and groups.</span></span>
4. <span data-ttu-id="fb7c3-118">Om du vill att en viss princip ska vara till för någon lägger du till honom eller honom i listan Med.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="fb7c3-119">För att säkerställa att en person utelämnas från principen lägger du till dem i listan med uteslutning.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="fb7c3-120">Användbara länkar:</span><span class="sxs-lookup"><span data-stu-id="fb7c3-120">Helpful links:</span></span>

[<span data-ttu-id="fb7c3-121">Översikt över enhetsefterlevnad</span><span class="sxs-lookup"><span data-stu-id="fb7c3-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="fb7c3-122">Felsökning av certifikatutfärdare</span><span class="sxs-lookup"><span data-stu-id="fb7c3-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="fb7c3-123">Felsökningsprincip</span><span class="sxs-lookup"><span data-stu-id="fb7c3-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="fb7c3-124">Övervaka Intune-enhetsefterlevnad</span><span class="sxs-lookup"><span data-stu-id="fb7c3-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="fb7c3-125">Obs! De här stegen är bara användbara vid felsökning av villkorsstyrd åtkomst i Azure Active Directory-funktionen.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="fb7c3-126">Det går även att sätta en enhet i karantän, så att den inte får åtkomst till e-post med Exchange-principen.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="fb7c3-127">Mer information om hantering av Exchange-enheter finns [här]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="fb7c3-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
