---
title: DLP-regel för kreditkortsnummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389595"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="32d5f-102">DLP-problem med kreditkortsnummer</span><span class="sxs-lookup"><span data-stu-id="32d5f-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="32d5f-103">Har du problem med **Data förlust Prevention (DLP)** fungerar inte för innehåll som innehåller ett **Kreditkortsnummer** när du använder en DLP känslig informationstyp i O365?</span><span class="sxs-lookup"><span data-stu-id="32d5f-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="32d5f-104">Om så är fallet, kontrollera innehållet innehåller informationen som krävs för att utlösa den DLP-principen när det utvärderas.</span><span class="sxs-lookup"><span data-stu-id="32d5f-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="32d5f-105">Till exempel ett **kreditkort princip** konfigureras med en konfidensnivå på 85%, följande utvärderas och måste identifieras att utlösa regeln:</span><span class="sxs-lookup"><span data-stu-id="32d5f-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="32d5f-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 siffror som kan vara formaterad eller oformaterad (dddddddddddddddd) och måste klara Luhn-testet.</span><span class="sxs-lookup"><span data-stu-id="32d5f-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="32d5f-107">**[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Mycket komplexa och robust mönster som identifierar kort från alla stora varumärken över hela världen, inklusive Visa, MasterCard, Discover-kort, JCB, American Express, presentkort och diner-kort.</span><span class="sxs-lookup"><span data-stu-id="32d5f-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="32d5f-108">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn-kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="32d5f-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="32d5f-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-princip är 85% säker på att den har upptäckt att den här typen av känslig information om inom ett avstånd av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="32d5f-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="32d5f-110">Funktionen Func_credit_card returnerar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="32d5f-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="32d5f-111">Något av följande är sant:</span><span class="sxs-lookup"><span data-stu-id="32d5f-111">One of the following is true:</span></span>

  - <span data-ttu-id="32d5f-112">Det finns ett nyckelord från Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="32d5f-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="32d5f-113">Ett nyckelord från Keyword_cc_name hittades</span><span class="sxs-lookup"><span data-stu-id="32d5f-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="32d5f-114">Funktionen Func_expiration_date söker efter ett datum i formatet rätt datum.</span><span class="sxs-lookup"><span data-stu-id="32d5f-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="32d5f-115">Kontrollsumman passerar</span><span class="sxs-lookup"><span data-stu-id="32d5f-115">The checksum passes</span></span>

    <span data-ttu-id="32d5f-116">Till exempel initierar i följande exempel principens DLP kreditkort nummer:</span><span class="sxs-lookup"><span data-stu-id="32d5f-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="32d5f-117">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="32d5f-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="32d5f-118">Förfaller: 2/2009</span><span class="sxs-lookup"><span data-stu-id="32d5f-118">Expires: 2/2009</span></span>

<span data-ttu-id="32d5f-119">Mer information om vad som krävs för ett **Kreditkortsnummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad den känsliga informationstyper leta efter kreditkort #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="32d5f-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="32d5f-120">Med en annan inbyggd känslig information-typ finns i följande artikel för information om vad som krävs för andra typer: [vad den känsliga informationstyper leta efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="32d5f-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  