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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366446"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="e2995-102">Övervaka villkorlig åtkomst för Exchange</span><span class="sxs-lookup"><span data-stu-id="e2995-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="e2995-103">Användare riktade mot villkorsstyrd åtkomst får ett e-postmeddelande om de inte uppfyller åtkomst kraven för organisationen.</span><span class="sxs-lookup"><span data-stu-id="e2995-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e2995-104">För att lösa problemet rekommenderar vi en eller flera av följande lösningar:</span><span class="sxs-lookup"><span data-stu-id="e2995-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="e2995-105">Om enheten är registrerad kan du uppmana användaren att gå till företagsportalsappen och kontrol lera att den visas i företags portalen.</span><span class="sxs-lookup"><span data-stu-id="e2995-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e2995-106">Om det inte gör det bör användaren registrera enheten.</span><span class="sxs-lookup"><span data-stu-id="e2995-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="e2995-107">I Azure-portalen går du till Intune > enhets efterlevnad.</span><span class="sxs-lookup"><span data-stu-id="e2995-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="e2995-108">Klicka på enhets överensstämmelse under bildskärm.</span><span class="sxs-lookup"><span data-stu-id="e2995-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="e2995-109">Visa din enhets kompatibilitetsstatus för att kontrol lera att användarens enhet är markerad som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="e2995-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="e2995-110">I Azure-portalen går du till Intune > enhets efterlevnad.</span><span class="sxs-lookup"><span data-stu-id="e2995-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="e2995-111">Under hantera klickar du på principer.</span><span class="sxs-lookup"><span data-stu-id="e2995-111">Under Manage, click Policies.</span></span> <span data-ttu-id="e2995-112">I listan över efterlevnadsprinciper kontrollerar du att en profil har tilldelats till din användares enhet.</span><span class="sxs-lookup"><span data-stu-id="e2995-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e2995-113">Om ingen profil är tilldelad kan Intune inte bekräfta status för enhetens efterlevnad.</span><span class="sxs-lookup"><span data-stu-id="e2995-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="e2995-114">Redigera användarens villkorliga åtkomst tilldelning.</span><span class="sxs-lookup"><span data-stu-id="e2995-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="e2995-115">I Azure-portalen går du till **Intune**  >  policy för**villkorlig åtkomst**  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="e2995-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="e2995-116">Välj en princip i listan.</span><span class="sxs-lookup"><span data-stu-id="e2995-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="e2995-117">Klicka på användare och grupper.</span><span class="sxs-lookup"><span data-stu-id="e2995-117">Click Users and groups.</span></span>
4. <span data-ttu-id="e2995-118">Om du vill rikta en viss princip till någon kan du lägga till dem i listan ta med.</span><span class="sxs-lookup"><span data-stu-id="e2995-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="e2995-119">Om du vill se till att en person utelämnas från policyn lägger du till den i listan undantag.</span><span class="sxs-lookup"><span data-stu-id="e2995-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="e2995-120">Användbara länkar:</span><span class="sxs-lookup"><span data-stu-id="e2995-120">Helpful links:</span></span>

[<span data-ttu-id="e2995-121">Översikt över enhetens efterlevnad</span><span class="sxs-lookup"><span data-stu-id="e2995-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="e2995-122">Felsöka CA</span><span class="sxs-lookup"><span data-stu-id="e2995-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="e2995-123">Fel söknings princip</span><span class="sxs-lookup"><span data-stu-id="e2995-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="e2995-124">Övervaka efterlevnad av Intune-enheter</span><span class="sxs-lookup"><span data-stu-id="e2995-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="e2995-125">Obs! de här stegen är bara till hjälp när du ska felsöka villkorlig åtkomst för Azure Active Directory-funktionen.</span><span class="sxs-lookup"><span data-stu-id="e2995-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="e2995-126">Det går också att använda karantän en enhet för att blockera e-poståtkomst med Exchange-princip.</span><span class="sxs-lookup"><span data-stu-id="e2995-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="e2995-127">Mer information om Exchange Device Management finns [här](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="e2995-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
