---
title: Prestandaproblem för Microsoft Defender för Slutpunkt i Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794225"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="f8ee7-102">Prestandaproblem för Microsoft Defender för Slutpunkt i Linux</span><span class="sxs-lookup"><span data-stu-id="f8ee7-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="f8ee7-103">Den här artikeln leder dig genom stegen för att identifiera prestandaproblem för Microsoft Defender för Endpoint på Linux.</span><span class="sxs-lookup"><span data-stu-id="f8ee7-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="f8ee7-104">Det är viktigt att du först kontrollerar att problemet är löst i den [senaste versionen.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="f8ee7-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="f8ee7-105">Information om hur du startar din undersökning [finns i Felsöka prestandaproblem för Microsoft Defender för Endpoint på Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="f8ee7-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="f8ee7-106">Undantag</span><span class="sxs-lookup"><span data-stu-id="f8ee7-106">Exclusions</span></span>

<span data-ttu-id="f8ee7-107">Undantag kan bidra till att minimera prestandaproblem.</span><span class="sxs-lookup"><span data-stu-id="f8ee7-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="f8ee7-108">Granska undantagen innan du börjar så att alla ytterligare risker är kända och har dokumenterats.</span><span class="sxs-lookup"><span data-stu-id="f8ee7-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="f8ee7-109">Mer information finns i [Konfigurera och validera undantag för Microsoft Defender för Endpoint på Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="f8ee7-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="f8ee7-110">När du har flera & mappar som ska undantas och de alla finns på samma monteringspunkt, kan det vara enklare att utesluta fästpunkten.</span><span class="sxs-lookup"><span data-stu-id="f8ee7-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="f8ee7-111">Från och med februari version 101.22.80 kan du utesluta en hel monteringspunkt.</span><span class="sxs-lookup"><span data-stu-id="f8ee7-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="f8ee7-112">Om till exempel /mnt/backup är en monteringspunkt kan du lägga till /mnt/backup i exkluderingslistan genom att köra det här kommandot:</span><span class="sxs-lookup"><span data-stu-id="f8ee7-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="f8ee7-113">**Obs!** Om du lägger till undantag ökar risken för att skadlig programvara inte identifieras och bör hanteras och implementeras med försiktighet.</span><span class="sxs-lookup"><span data-stu-id="f8ee7-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="f8ee7-114">Behöver du hjälp?</span><span class="sxs-lookup"><span data-stu-id="f8ee7-114">Need Help?</span></span>

<span data-ttu-id="f8ee7-115">Samla in diagnostikdata innan du öppnar ett supportfall för att hjälpa dig på det mest effektiva sättet.</span><span class="sxs-lookup"><span data-stu-id="f8ee7-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
