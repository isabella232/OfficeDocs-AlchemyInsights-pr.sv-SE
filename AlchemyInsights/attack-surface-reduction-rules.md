---
title: Regler för minskning av attackytan
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676444"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="07e34-102">Regler för minskning av attackytan</span><span class="sxs-lookup"><span data-stu-id="07e34-102">Attack surface reduction rules</span></span>

<span data-ttu-id="07e34-103">Att utesluta filer eller mappar kan allvarligt minska skyddet som tillhandahålls av minskningsregler för attackytan.</span><span class="sxs-lookup"><span data-stu-id="07e34-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="07e34-104">Filer som skulle ha blockerats av en regel tillåts köras och ingen rapport eller händelse registreras.</span><span class="sxs-lookup"><span data-stu-id="07e34-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="07e34-105">Ett undantag gäller för alla regler som tillåter undantag.</span><span class="sxs-lookup"><span data-stu-id="07e34-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="07e34-106">ASR-undantag använder samma syntax som Microsoft Defender Antivirus undantag.</span><span class="sxs-lookup"><span data-stu-id="07e34-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="07e34-107">Mer information finns i [Konfigurera och validera undantag för Microsoft Defender Antivirus genomsökningar](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="07e34-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="07e34-108">Om du vill undvika problem [kan du läsa vanliga misstag som du bör undvika när du definierar undantag](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="07e34-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="07e34-109">Alla ASR-regler stöder inte undantag.</span><span class="sxs-lookup"><span data-stu-id="07e34-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="07e34-110">Information om hur du kontrollerar om regeln stöder undantag finns i tabellen [Minskning av attackytan](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="07e34-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="07e34-111">Regler för minskning av attackytan</span><span class="sxs-lookup"><span data-stu-id="07e34-111">Attack surface reduction rules</span></span>

<span data-ttu-id="07e34-112">Din organisations attackyta omfattar alla platser där en attack kan avslöja organisationsenheter eller nätverk.</span><span class="sxs-lookup"><span data-stu-id="07e34-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="07e34-113">Att minska attackytan innebär att skydda organisationens enheter och nätverk, vilket lämnar attacker med färre sätt att utföra attacker.</span><span class="sxs-lookup"><span data-stu-id="07e34-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="07e34-114">Det kan hjälpa att konfigurera regler för att minska attackytan i Microsoft Defender för Endpoint.</span><span class="sxs-lookup"><span data-stu-id="07e34-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="07e34-115">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="07e34-115">For more information, see:</span></span>

- [<span data-ttu-id="07e34-116">Mappa ASR-regel-GUID till namn</span><span class="sxs-lookup"><span data-stu-id="07e34-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="07e34-117">Krav för ASR-regler:</span><span class="sxs-lookup"><span data-stu-id="07e34-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="07e34-118">Windows 10 Pro, version 1709 eller senare</span><span class="sxs-lookup"><span data-stu-id="07e34-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="07e34-119">Windows 10 Enterprise, version 1709 eller senare</span><span class="sxs-lookup"><span data-stu-id="07e34-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="07e34-120">Windows Server, version 1803 (Halvårskanal) eller senare</span><span class="sxs-lookup"><span data-stu-id="07e34-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="07e34-121">Identifiera rätt undantag som ska tillämpas</span><span class="sxs-lookup"><span data-stu-id="07e34-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="07e34-122">Leta efter eventID 1121 eller 1122 i Microsoft-Windows-Windows Defender/Operational-loggen.</span><span class="sxs-lookup"><span data-stu-id="07e34-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="07e34-123">Utvärdera blockeringsscenariot och -kontexten och bekräfta att det här scenariot måste avblockas.</span><span class="sxs-lookup"><span data-stu-id="07e34-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="07e34-124">Läs värdet Path i händelseinformationen, som är det värde som definierar undantaget.</span><span class="sxs-lookup"><span data-stu-id="07e34-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="07e34-125">Se till att undantaget är så strikt som möjligt.</span><span class="sxs-lookup"><span data-stu-id="07e34-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="07e34-126">Använd ett jokertecken när det behövs (t.ex. ersätt användarvariabel).</span><span class="sxs-lookup"><span data-stu-id="07e34-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="07e34-127">Tillämpa undantaget enligt dina behov vid distribution.</span><span class="sxs-lookup"><span data-stu-id="07e34-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="07e34-128">Mer information finns i [Anpassa regler för att minska attackytan.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="07e34-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="07e34-129">Undantag respekteras inte</span><span class="sxs-lookup"><span data-stu-id="07e34-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="07e34-130">Bestäm om regeln ska stödja undantag.</span><span class="sxs-lookup"><span data-stu-id="07e34-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="07e34-131">Mer information finns i Regler [för att minska attackytan.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="07e34-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="07e34-132">Granska undantag som tillämpas och verifiera med händelsedata för skrivfel eller felupptecknade jokertecken.</span><span class="sxs-lookup"><span data-stu-id="07e34-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="07e34-133">Mer information finns i [Undantagstyper som stöds](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="07e34-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="07e34-134">Om effekten av regeln är för hög kan du flytta tillbaka regeln (tillbaka) till granskningsläge för ytterligare validering.</span><span class="sxs-lookup"><span data-stu-id="07e34-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="07e34-135">Mer information finns i [Testa hur Microsoft Defender för slutpunktsfunktioner fungerar i granskningsläge.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="07e34-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="07e34-136">Samla in supportdata för att öppna ett supportfall med hjälp av det här kommandot:</span><span class="sxs-lookup"><span data-stu-id="07e34-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="07e34-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="07e34-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="07e34-138">Mer information finns i Problem [med onboarding-datorer till Microsoft Defender för slutpunkter.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="07e34-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
