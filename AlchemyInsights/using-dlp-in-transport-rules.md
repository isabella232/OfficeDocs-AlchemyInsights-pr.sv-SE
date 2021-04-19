---
title: Använda DLP i transportregler
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827234"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="8322b-102">Använda DLP i transportregler</span><span class="sxs-lookup"><span data-stu-id="8322b-102">Using DLP in transport rules</span></span>

<span data-ttu-id="8322b-103">Om du vill integrera skydd mot dataförlust (DLP) i en befintlig transport använder du villkoret "**om meddelandet innehåller...Känslig information**" i inställningarna för transportregel.</span><span class="sxs-lookup"><span data-stu-id="8322b-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="8322b-104">**Mer information finns i:**</span><span class="sxs-lookup"><span data-stu-id="8322b-104">**For more details, see:**</span></span>

- <span data-ttu-id="8322b-105">Integrerade DLP känsliga informationstyper i transportregler: [Integrera känslig information-regler](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="8322b-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="8322b-106">Du kan även testa regeln med eller utan policytest med hjälp av testläget för regeln.</span><span class="sxs-lookup"><span data-stu-id="8322b-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="8322b-107">Du bör vänta 30 minuter efter att ha skapat regeln innan du testar den.</span><span class="sxs-lookup"><span data-stu-id="8322b-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="8322b-108">Mer hittar du i [ Testa e-postflödes-/transportregler](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="8322b-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="8322b-109">**Obs**: om du försöker implementera en ny DLP-princip med transportregler i EAC ska du använda [DLP-principer i säkerhets- och efterlevnadscenter](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) i stället.</span><span class="sxs-lookup"><span data-stu-id="8322b-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
