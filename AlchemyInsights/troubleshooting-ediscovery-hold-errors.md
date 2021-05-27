---
title: Felsökning av ediscovery som innehåller fel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676284"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="7306a-102">Felsökning av ediscovery som innehåller fel</span><span class="sxs-lookup"><span data-stu-id="7306a-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="7306a-103">Har du problem med eDiscovery-eDiscovery-rymmer?</span><span class="sxs-lookup"><span data-stu-id="7306a-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="7306a-104">Här är några metodtips att tänka på:</span><span class="sxs-lookup"><span data-stu-id="7306a-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="7306a-105">Kontrollera statusen för statusen för håll distribution.</span><span class="sxs-lookup"><span data-stu-id="7306a-105">Check the hold distribution status.</span></span>  <span data-ttu-id="7306a-106">Om statusen **är På (Väntande)** **eller Av (Väntande)** väntar du på att distributionen för väntande är slutförd.</span><span class="sxs-lookup"><span data-stu-id="7306a-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="7306a-107">Koppla eDiscovery och håll uppdateringar i en enda massbegäran i stället för att uppdatera principen flera gånger för varje transaktion.</span><span class="sxs-lookup"><span data-stu-id="7306a-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="7306a-108">Kör Set-CaseHoldPolicy <policyname> -RetryDistribution i Säkerhets- och efterlevnadscenter Powershell.</span><span class="sxs-lookup"><span data-stu-id="7306a-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="7306a-109">Mer information finns i [Anslut säkerhets- och & PowerShell.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="7306a-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="7306a-110">Anvisningar för hur du kontrollerar de här inställningarna och ytterligare metodtips för att minska och åtgärda eDiscovery-problem som kan innehålla problem finns i [Felsöka fel för eDiscovery-spärrade e-dataidentifiering.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="7306a-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="7306a-111">Mer information om felsökning av andra vanliga eDiscovery-problem finns i [Undersöka, felsöka och lösa vanliga eDiscovery-problem.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="7306a-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
