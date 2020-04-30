---
title: Använda DLP i transportregler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915296"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="666eb-102">Använda DLP i transportregler</span><span class="sxs-lookup"><span data-stu-id="666eb-102">Using DLP in transport rules</span></span>

<span data-ttu-id="666eb-103">Om du vill integrera skydd mot dataförlust (DLP) i en befintlig transport använder du villkoret "**om meddelandet innehåller...Känslig information**" i inställningarna för transportregel.</span><span class="sxs-lookup"><span data-stu-id="666eb-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="666eb-104">**Mer information finns i:**</span><span class="sxs-lookup"><span data-stu-id="666eb-104">**For more details, see:**</span></span>

- <span data-ttu-id="666eb-105">Integrerade DLP känsliga informationstyper i transportregler: [Integrera känslig information-regler](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="666eb-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="666eb-106">Du kan även testa regeln med eller utan policytest med hjälp av testläget för regeln.</span><span class="sxs-lookup"><span data-stu-id="666eb-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="666eb-107">Du bör vänta 30 minuter efter att ha skapat regeln innan du testar den.</span><span class="sxs-lookup"><span data-stu-id="666eb-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="666eb-108">Mer hittar du i [ Testa e-postflödes-/transportregler](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="666eb-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="666eb-109">**Obs**: om du försöker implementera en ny DLP-princip med transportregler i EAC ska du använda [DLP-principer i säkerhets- och efterlevnadscenter](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stället.</span><span class="sxs-lookup"><span data-stu-id="666eb-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
