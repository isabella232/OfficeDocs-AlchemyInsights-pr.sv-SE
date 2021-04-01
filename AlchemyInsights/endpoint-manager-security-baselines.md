---
title: EndPoint Manager – Säkerhetsbaslinjer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440911"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="a539c-102">EndPoint Manager – Säkerhetsbaslinjer</span><span class="sxs-lookup"><span data-stu-id="a539c-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="a539c-103">Säkerhetsbaslinjer är förkonfigurerade grupper med Windows-inställningar som hjälper dig att använda de säkerhetsinställningar som rekommenderas av relevanta säkerhetsteam.</span><span class="sxs-lookup"><span data-stu-id="a539c-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="a539c-104">Dessa baslinjer kan anpassas så att endast önskade inställningar och värden levereras.</span><span class="sxs-lookup"><span data-stu-id="a539c-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="a539c-105">Mer information om säkerhetsbaslinjer finns i [Använda säkerhetsbaslinjer för att konfigurera Windows 10-enheter i Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="a539c-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="a539c-106">Det finns för närvarande baslinjer för dessa produkter:</span><span class="sxs-lookup"><span data-stu-id="a539c-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="a539c-107">Säkerhetsinställningar för Windows MDM</span><span class="sxs-lookup"><span data-stu-id="a539c-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="a539c-108">Säkerhet för Microsoft Defender för Endpoint</span><span class="sxs-lookup"><span data-stu-id="a539c-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="a539c-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a539c-109">Microsoft Edge</span></span>

<span data-ttu-id="a539c-110">Alla baslinjer uppdateras regelbundet och publiceras i stegvisa versioner.</span><span class="sxs-lookup"><span data-stu-id="a539c-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="a539c-111">Varje version lägger till och tar bort inställningar från den tidigare versionen för att säkerställa att baslinjen uppfyller aktuella riktlinjer.</span><span class="sxs-lookup"><span data-stu-id="a539c-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="a539c-112">Med säkerhetsbaslinjekonsolen i Endpoint-säkerhet kan olika versioner jämföras genom att göra ändringarna från version till version synliga.</span><span class="sxs-lookup"><span data-stu-id="a539c-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="a539c-113">Mer information om hur du bäst ändrar vilken version av baslinjen som distribueras finns i [Hantera säkerhetsbaslinjeprofiler i Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="a539c-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="a539c-114">När du har distribuerat en säkerhetsbaslinje kan du övervaka distributionstillståndet och granska inställningarna för varje enhet.</span><span class="sxs-lookup"><span data-stu-id="a539c-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="a539c-115">**Obs!** Det kan ta upp till 24 timmar innan rapporteringsdata för baslinjer visas från den första distributionen till en enhet och upp till 6 timmar för ytterligare uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="a539c-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="a539c-116">Den vanligaste orsaken till att en baslinjeinställning inte används är att samma inställning används i en annan profil.</span><span class="sxs-lookup"><span data-stu-id="a539c-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="a539c-117">Det här scenariot kan undersökas för specifika enheter genom att välja enheten i noden Enhetsstatus i profilen Säkerhetsbaslinje.</span><span class="sxs-lookup"><span data-stu-id="a539c-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="a539c-118">Mer information finns i [Lösa konflikter för säkerhetsbaslinjer](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="a539c-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>