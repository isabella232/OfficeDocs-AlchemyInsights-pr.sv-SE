---
title: EndPoint Manager – baslinjer för säkerhet
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
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421092"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="3358e-102">EndPoint Manager – baslinjer för säkerhet</span><span class="sxs-lookup"><span data-stu-id="3358e-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="3358e-103">Säkerhetsbaslinjer är förkonfigurerade grupper med Windows-inställningar som hjälper dig att tillämpa de säkerhetsinställningar som rekommenderas av relevanta säkerhetsteam.</span><span class="sxs-lookup"><span data-stu-id="3358e-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="3358e-104">Dessa baslinjer kan anpassas så att de bara ger de inställningar och värden du önskar.</span><span class="sxs-lookup"><span data-stu-id="3358e-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="3358e-105">Mer information om säkerhetsbaslinjer finns i Använda [säkerhetsbaslinjer för att konfigurera Windows 10-enheter i Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="3358e-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="3358e-106">Det finns för närvarande baslinjer för dessa produkter:</span><span class="sxs-lookup"><span data-stu-id="3358e-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="3358e-107">Inställningar för Windows MDM-säkerhet</span><span class="sxs-lookup"><span data-stu-id="3358e-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="3358e-108">Microsoft Defender för EndPoint-säkerhet</span><span class="sxs-lookup"><span data-stu-id="3358e-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="3358e-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="3358e-109">Microsoft Edge</span></span>

<span data-ttu-id="3358e-110">Alla baslinjer uppdateras regelbundet och släpps i stegvisa versioner.</span><span class="sxs-lookup"><span data-stu-id="3358e-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="3358e-111">Varje version lägger till och tar bort inställningar från den föregående versionen för att säkerställa att baslinjen uppfyller aktuella riktlinjer.</span><span class="sxs-lookup"><span data-stu-id="3358e-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="3358e-112">Med konsolen säkerhetsbaslinjer i Slutpunktssäkerhet kan olika versioner jämföras genom att ändringarna från version till version blir synliga.</span><span class="sxs-lookup"><span data-stu-id="3358e-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="3358e-113">Information om hur du på effektivast sätt ändrar vilken version av originalplan som distribueras finns i Hantera profiler för [säkerhetsbaslinje i Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="3358e-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="3358e-114">När du har distribuerat en säkerhetsbaslinje kan du övervaka statusen för distributionen och granska inställningarna enhet för enhet.</span><span class="sxs-lookup"><span data-stu-id="3358e-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="3358e-115">**Obs!** Det kan ta upp till 24 timmar innan rapportdata för baslinjer visas från den första distributionen till en enhet och upp till 6 timmar för ytterligare uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="3358e-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="3358e-116">Den vanligaste orsaken till att en baslinjeinställning inte används är att samma inställning används i en annan profil.</span><span class="sxs-lookup"><span data-stu-id="3358e-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="3358e-117">Det här scenariot kan undersökas för specifik enhet genom att välja enheten från noden Enhetsstatus i profilen Baslinje för säkerhet.</span><span class="sxs-lookup"><span data-stu-id="3358e-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="3358e-118">Mer information finns i [Lösa konflikter för säkerhetsbaslinjer.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="3358e-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>