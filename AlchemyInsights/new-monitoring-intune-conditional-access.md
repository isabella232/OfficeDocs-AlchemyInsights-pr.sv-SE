---
title: Övervaka villkorsstyrd Intune-åtkomst
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428308"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="e56fa-102">Övervaka villkorsstyrd Intune-åtkomst</span><span class="sxs-lookup"><span data-stu-id="e56fa-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="e56fa-103">Användare med villkorsstyrd åtkomst får ett e-postmeddelande om de inte uppfyller organisationens åtkomstkrav.</span><span class="sxs-lookup"><span data-stu-id="e56fa-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e56fa-104">Som lösning på det rekommenderar vi en eller flera av följande lösningar:</span><span class="sxs-lookup"><span data-stu-id="e56fa-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="e56fa-105">Om enheten antas vara registrerad kan du be användaren gå till företagsportalappen och kontrollera att den visas i företagsportalen.</span><span class="sxs-lookup"><span data-stu-id="e56fa-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e56fa-106">Om den inte gör det måste användaren registrera enheten.</span><span class="sxs-lookup"><span data-stu-id="e56fa-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="e56fa-107">Gå till **Intune-enhetsefterlevnad i**  >  **Azure-portalen.**</span><span class="sxs-lookup"><span data-stu-id="e56fa-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="e56fa-108">Om du vill visa rapporten över enhetsefterlevnad och verifiera att användarens enhet är markerad som kompatibel klickar du **på** Enhetsefterlevnad under **Bildskärm.**</span><span class="sxs-lookup"><span data-stu-id="e56fa-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="e56fa-109">Gå till **Intune-enhetsefterlevnad i**  >  **Azure-portalen.**</span><span class="sxs-lookup"><span data-stu-id="e56fa-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="e56fa-110">Klicka **på Principer under** **Hantera.**</span><span class="sxs-lookup"><span data-stu-id="e56fa-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="e56fa-111">Kontrollera att en profil är tilldelad till användarens enhet i listan över efterlevnadsprinciper.</span><span class="sxs-lookup"><span data-stu-id="e56fa-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e56fa-112">Om ingen profil har tilldelats kan Intune inte bekräfta enhetens efterlevnadsstatus.</span><span class="sxs-lookup"><span data-stu-id="e56fa-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="e56fa-113">Redigera användarens tilldelning av villkorsstyrd åtkomst.</span><span class="sxs-lookup"><span data-stu-id="e56fa-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="e56fa-114">Gå till Villkorsstyrda åtkomstprinciper för **Intune** i Azure-portalen, välj en princip i listan  >    >  och klicka **på Användare och grupper.**</span><span class="sxs-lookup"><span data-stu-id="e56fa-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="e56fa-115">Om du vill att en viss princip ska vara till för någon lägger du till honom eller honom i **listan Med.**</span><span class="sxs-lookup"><span data-stu-id="e56fa-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="e56fa-116">Om du vill säkerställa att en person utelämnas från principen lägger du till dem i **listan med uteslutning.**</span><span class="sxs-lookup"><span data-stu-id="e56fa-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="e56fa-117">**Användbara länkar:**</span><span class="sxs-lookup"><span data-stu-id="e56fa-117">**Helpful links:**</span></span>

- [<span data-ttu-id="e56fa-118">Översikt över enhetsefterlevnad</span><span class="sxs-lookup"><span data-stu-id="e56fa-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="e56fa-119">Felsökning av certifikatutfärdare</span><span class="sxs-lookup"><span data-stu-id="e56fa-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="e56fa-120">Felsökningsprincip</span><span class="sxs-lookup"><span data-stu-id="e56fa-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="e56fa-121">Övervaka Intune-enhetsefterlevnad</span><span class="sxs-lookup"><span data-stu-id="e56fa-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="e56fa-122">De här stegen är bara användbara när du felsöker Azure Active Directory-funktionen Villkorlig åtkomst.</span><span class="sxs-lookup"><span data-stu-id="e56fa-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="e56fa-123">Det går även att sätta en enhet i karantän, så att den inte har tillgång till e-post med Exchange-principen.</span><span class="sxs-lookup"><span data-stu-id="e56fa-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="e56fa-124">Mer information om hantering av Exchange-enheter finns [**här.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="e56fa-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
