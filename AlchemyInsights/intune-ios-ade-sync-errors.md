---
title: Automatiska synkroniseringsfel för automatisk enhets registrering
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714974"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="a2891-102">Automatiska synkroniseringsfel för automatisk enhets registrering</span><span class="sxs-lookup"><span data-stu-id="a2891-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="a2891-103">"Vi har upptäckt att du har en eller flera ADE-token i ett fel tillstånd.</span><span class="sxs-lookup"><span data-stu-id="a2891-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="a2891-104">Tills felet är löst för varje token fungerar inte ADE-funktionen för samma ".</span><span class="sxs-lookup"><span data-stu-id="a2891-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="a2891-105">Det här felet kan uppstå på flera olika sätt:</span><span class="sxs-lookup"><span data-stu-id="a2891-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="a2891-106">Enheter kan inte synkroniseras från ABM/ASM till Intune</span><span class="sxs-lookup"><span data-stu-id="a2891-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="a2891-107">Profil tilldelningar kan Miss lyckas</span><span class="sxs-lookup"><span data-stu-id="a2891-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="a2891-108">Enheter kan inte slutföra en ofullständig ADE-registrering</span><span class="sxs-lookup"><span data-stu-id="a2891-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="a2891-109">Kontrol lera det synkroniseringsfel som rapporter ATS i Intune-konsolen under **enheter > registrera enheter > > Apples registrerings program** och granska följande dokumentation för att se eventuell reparation:</span><span class="sxs-lookup"><span data-stu-id="a2891-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="a2891-110">ABM/ASM sync-fel för iOS/iPad och macOS automatisk enhets registrerings-token</span><span class="sxs-lookup"><span data-stu-id="a2891-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
