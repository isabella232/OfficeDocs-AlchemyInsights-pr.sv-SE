---
title: Indikatorer fungerar inte med webbläsaren Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676468"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="8f62c-102">Indikatorer fungerar inte med webbläsaren Edge</span><span class="sxs-lookup"><span data-stu-id="8f62c-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="8f62c-103">När du har skapat en indikator så används den inte av Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="8f62c-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="8f62c-104">Mer information finns i [Skapa indikatorer för IP-adresser och URL:er/domäner.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="8f62c-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="8f62c-105">Steg 1: Kontrollera följande</span><span class="sxs-lookup"><span data-stu-id="8f62c-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="8f62c-106">Kontrollera att indikatorn är korrekt (inga stavfel i IP/URL, rätt åtgärd och rätt RBAC-grupper).</span><span class="sxs-lookup"><span data-stu-id="8f62c-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="8f62c-107">Vänta i minst 2 timmar efter att indikatorn har skapats för att ta hänsyn till eventuell fördröjning.</span><span class="sxs-lookup"><span data-stu-id="8f62c-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="8f62c-108">Kontrollera att systemet/systemerna är onboarded to Microsoft Defender för Endpoint.</span><span class="sxs-lookup"><span data-stu-id="8f62c-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="8f62c-109">Kontrollera att system kan kommunicera med molnet.</span><span class="sxs-lookup"><span data-stu-id="8f62c-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="8f62c-110">Kontrollera att Smartscreen är aktiverat och kan nås genom att gå till [testwebbplatsen](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="8f62c-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="8f62c-111">Steg 2: Felsöka det möjliga problemet</span><span class="sxs-lookup"><span data-stu-id="8f62c-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="8f62c-112">Kontrollera att klienten uppfyller kraven.</span><span class="sxs-lookup"><span data-stu-id="8f62c-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="8f62c-113">Mer information finns i [Skapa indikatorer för IP-adresser och URL:er/domäner.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="8f62c-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="8f62c-114">Kontrollera att du kör den senaste versionen av Webbläsaren Edge.</span><span class="sxs-lookup"><span data-stu-id="8f62c-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="8f62c-115">Information om hur du tar reda på den senaste [versionen finns i Ta reda på vilken version Microsoft Edge du har](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="8f62c-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="8f62c-116">Starta om Webbläsaren Edge.</span><span class="sxs-lookup"><span data-stu-id="8f62c-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="8f62c-117">Navigera till den webbplats där du har gjort en indikator.</span><span class="sxs-lookup"><span data-stu-id="8f62c-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="8f62c-118">Om webbplatsen inte visas som förväntat fortsätter du till steg 3.</span><span class="sxs-lookup"><span data-stu-id="8f62c-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="8f62c-119">Steg 3: Samla in data</span><span class="sxs-lookup"><span data-stu-id="8f62c-119">Step 3: Collect data</span></span>

- <span data-ttu-id="8f62c-120">Samla **in diagnostikdata från MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="8f62c-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="8f62c-121">Anvisningar finns i Problem [med onboarding-datorer till Microsoft Defender för Endpoint.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="8f62c-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="8f62c-122">Om du är bekväm med att installera och samla in en Fiddler-spårning kan du gå [till Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="8f62c-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="8f62c-123">Om du föredrar vägledning från Microsoft Support väljer du ikonen Support nedan för att öppna ett supportfall.</span><span class="sxs-lookup"><span data-stu-id="8f62c-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
