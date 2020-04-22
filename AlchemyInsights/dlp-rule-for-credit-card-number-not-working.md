---
title: DLP-regeln för kreditkortsnummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704219"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="b01cb-102">DLP-problem med kreditkortsnummer</span><span class="sxs-lookup"><span data-stu-id="b01cb-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="b01cb-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="b01cb-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b01cb-104">**DLP-problem med kreditkortsnummer**</span><span class="sxs-lookup"><span data-stu-id="b01cb-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="b01cb-105">Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett **kreditkortsnummer** när du använder en DLP-känslig informationstyp i O365?</span><span class="sxs-lookup"><span data-stu-id="b01cb-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="b01cb-106">Om så är fallet, se till att ditt innehåll innehåller den information som behövs för att utlösa DLP-principen när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="b01cb-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="b01cb-107">För en **kreditkortsprincip** som konfigurerats med en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:</span><span class="sxs-lookup"><span data-stu-id="b01cb-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="b01cb-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 siffror som kan formateras eller oformateras (ddddddddddddddddd) och måste klara Luhn-testet.</span><span class="sxs-lookup"><span data-stu-id="b01cb-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="b01cb-109">**[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Mycket komplext och robust mönster som upptäcker kort från alla större märken över hela världen, inklusive Visa, MasterCard, Discover Card, JCB, American Express, presentkort och dinerkort.</span><span class="sxs-lookup"><span data-stu-id="b01cb-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="b01cb-110">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn checksum</span><span class="sxs-lookup"><span data-stu-id="b01cb-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="b01cb-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-princip är 85 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="b01cb-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="b01cb-112">Funktionen Func_credit_card hittar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="b01cb-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="b01cb-113">Ett av följande gäller:</span><span class="sxs-lookup"><span data-stu-id="b01cb-113">One of the following is true:</span></span>

  - <span data-ttu-id="b01cb-114">Ett nyckelord från Keyword_cc_verification hittas.</span><span class="sxs-lookup"><span data-stu-id="b01cb-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="b01cb-115">Ett nyckelord från Keyword_cc_name hittas</span><span class="sxs-lookup"><span data-stu-id="b01cb-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="b01cb-116">Funktionen Func_expiration_date hittar ett datum i rätt datumformat.</span><span class="sxs-lookup"><span data-stu-id="b01cb-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="b01cb-117">Kontrollsumman passerar</span><span class="sxs-lookup"><span data-stu-id="b01cb-117">The checksum passes</span></span>

    <span data-ttu-id="b01cb-118">Följande exempel skulle till exempel utlösa för en DLP-kreditkortsnummerpolicy:</span><span class="sxs-lookup"><span data-stu-id="b01cb-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="b01cb-119">Visum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="b01cb-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="b01cb-120">Löper ut: 2/2009</span><span class="sxs-lookup"><span data-stu-id="b01cb-120">Expires: 2/2009</span></span>

<span data-ttu-id="b01cb-121">Mer information om vad som krävs för att ett **kreditkortsnummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter kreditkort#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="b01cb-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="b01cb-122">Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="b01cb-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  