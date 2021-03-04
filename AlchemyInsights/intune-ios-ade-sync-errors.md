---
title: Synkroniseringsfel för automatisk enhetsregistrering för Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448940"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="b351a-102">Synkroniseringsfel för automatisk enhetsregistrering för Apple</span><span class="sxs-lookup"><span data-stu-id="b351a-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="b351a-103">"Vi har upptäckt att du har en eller flera ADE/DEP-token som är i ett felläge.</span><span class="sxs-lookup"><span data-stu-id="b351a-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="b351a-104">Tills feltillståndet har lösts för varje påverkad token fungerar inte ADE-funktionerna som förväntat."</span><span class="sxs-lookup"><span data-stu-id="b351a-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="b351a-105">Det här felet kan visa sig på flera olika sätt, bland annat:</span><span class="sxs-lookup"><span data-stu-id="b351a-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="b351a-106">Enheter kan inte synkronisera från ABM/ASM till Intune</span><span class="sxs-lookup"><span data-stu-id="b351a-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="b351a-107">Profiltilldelningar i registrering kanske inte fungerar</span><span class="sxs-lookup"><span data-stu-id="b351a-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="b351a-108">Enheter kanske inte slutför ADE-registreringen</span><span class="sxs-lookup"><span data-stu-id="b351a-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="b351a-109">Kontrollera om synkroniseringsfelet har rapporterats på Intune-konsolen under Enheter > Registrera enheter **> Apple-registrering > token för registreringsprogram.**</span><span class="sxs-lookup"><span data-stu-id="b351a-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="b351a-110">En av de vanligaste orsakerna till synkroniseringsfel är att den aktuella tokenet förfaller.</span><span class="sxs-lookup"><span data-stu-id="b351a-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="b351a-111">I många fall löser förnyelsen av den aktuella tokenen problemet.</span><span class="sxs-lookup"><span data-stu-id="b351a-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="b351a-112">Om en eller flera av dina token har upphört att gälla kan du läsa följande dokumentation som hjälper dig att förnya dem efter behov:</span><span class="sxs-lookup"><span data-stu-id="b351a-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="b351a-113">Förnya en token för automatisk enhetsregistrering</span><span class="sxs-lookup"><span data-stu-id="b351a-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="b351a-114">Dessutom kan du se följande dokumentation för att se möjliga åtgärder för andra fel som orsakar tokensynkroniseringsfel:</span><span class="sxs-lookup"><span data-stu-id="b351a-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="b351a-115">ABM-/ASM-synkroniseringsfel för iOS-/iPadOS- och macOS-token för automatisk enhetsregistrering</span><span class="sxs-lookup"><span data-stu-id="b351a-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="b351a-116">ABM-/ASM-synkroniseringsfel för iOS-/iPadOS- och macOS-token för automatisk enhetsregistrering</span><span class="sxs-lookup"><span data-stu-id="b351a-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
