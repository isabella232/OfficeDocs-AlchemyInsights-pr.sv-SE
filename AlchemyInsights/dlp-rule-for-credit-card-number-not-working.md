---
title: DLP-regel för kreditkorts nummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679459"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="18beb-102">DLP-problem med kreditkorts nummer</span><span class="sxs-lookup"><span data-stu-id="18beb-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="18beb-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="18beb-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="18beb-104">**DLP-problem med kreditkorts nummer**</span><span class="sxs-lookup"><span data-stu-id="18beb-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="18beb-105">Har du problem med **data förlust skydd (DLP)** fungerar inte för innehåll som innehåller ett **kreditkorts nummer** när du använder en DLP-känslig informations typ i O365?</span><span class="sxs-lookup"><span data-stu-id="18beb-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="18beb-106">Om så är fallet kontrollerar du att innehållet innehåller den information som behövs för att utlösa DLP-principen när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="18beb-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="18beb-107">För att en **kredit korts princip** är konfigurerad med en konfidensnivå på 85% utvärderas till exempel följande och måste identifieras för att regeln ska utlösa:</span><span class="sxs-lookup"><span data-stu-id="18beb-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="18beb-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 siffror som kan formateras eller formateras (ssssssssssssssss) och måste godkänna Luhn-testet.</span><span class="sxs-lookup"><span data-stu-id="18beb-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="18beb-109">**[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Mycket komplext och robust mönster som identifierar kort från alla större varumärken, inklusive Visa, MasterCard, Discover-kort, JCB, American Express, presentkort och betalkort-kort.</span><span class="sxs-lookup"><span data-stu-id="18beb-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="18beb-110">**[Kontroll Summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn, kontroll Summa</span><span class="sxs-lookup"><span data-stu-id="18beb-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="18beb-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-princip är 85% trygg att den här typen av känslig information identifieras om, inom ett avstånd på 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="18beb-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="18beb-112">Funktionen Func_credit_card hittar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="18beb-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="18beb-113">Något av följande stämmer:</span><span class="sxs-lookup"><span data-stu-id="18beb-113">One of the following is true:</span></span>

  - <span data-ttu-id="18beb-114">Ett nyckelord från Keyword_cc_verification hittas.</span><span class="sxs-lookup"><span data-stu-id="18beb-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="18beb-115">Ett nyckelord från Keyword_cc_name hittas</span><span class="sxs-lookup"><span data-stu-id="18beb-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="18beb-116">Funktionen Func_expiration_date hittar ett datum i rätt datum format.</span><span class="sxs-lookup"><span data-stu-id="18beb-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="18beb-117">Kontroll summan passerar</span><span class="sxs-lookup"><span data-stu-id="18beb-117">The checksum passes</span></span>

    <span data-ttu-id="18beb-118">Följande exempel skulle till exempel utlösa en policy för DLP-kreditkorts nummer:</span><span class="sxs-lookup"><span data-stu-id="18beb-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="18beb-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="18beb-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="18beb-120">Upphör: 2/2009</span><span class="sxs-lookup"><span data-stu-id="18beb-120">Expires: 2/2009</span></span>

<span data-ttu-id="18beb-121">Mer information om vad som krävs för att ett **kreditkorts nummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [vad den känsliga informations typen letar efter kreditkort #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="18beb-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="18beb-122">Om du använder en annan inbyggd känslig informations typ kan du läsa följande artikel för information om vad som är obligatoriskt för andra typer: [vad den känsliga informations typen letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="18beb-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  