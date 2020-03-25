---
title: DLP-regeln för kreditkortsnummer fungerar inte
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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932461"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="7b064-102">DLP-problem med kreditkortsnummer</span><span class="sxs-lookup"><span data-stu-id="7b064-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="7b064-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="7b064-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7b064-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="7b064-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7b064-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="7b064-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7b064-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="7b064-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7b064-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="7b064-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7b064-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="7b064-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7b064-109">**DLP-problem med kreditkortsnummer**</span><span class="sxs-lookup"><span data-stu-id="7b064-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="7b064-110">Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett **kreditkortsnummer** när du använder en DLP-känslig informationstyp i O365?</span><span class="sxs-lookup"><span data-stu-id="7b064-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="7b064-111">Om så är fallet, se till att ditt innehåll innehåller den information som behövs för att utlösa DLP-principen när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="7b064-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="7b064-112">För en **kreditkortsprincip** som konfigurerats med en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:</span><span class="sxs-lookup"><span data-stu-id="7b064-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="7b064-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 siffror som kan formateras eller oformateras (ddddddddddddddddd) och måste klara Luhn-testet.</span><span class="sxs-lookup"><span data-stu-id="7b064-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="7b064-114">**[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Mycket komplext och robust mönster som upptäcker kort från alla större märken över hela världen, inklusive Visa, MasterCard, Discover Card, JCB, American Express, presentkort och dinerkort.</span><span class="sxs-lookup"><span data-stu-id="7b064-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="7b064-115">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn checksum</span><span class="sxs-lookup"><span data-stu-id="7b064-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="7b064-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-princip är 85 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="7b064-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="7b064-117">Funktionen Func_credit_card hittar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="7b064-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="7b064-118">Ett av följande gäller:</span><span class="sxs-lookup"><span data-stu-id="7b064-118">One of the following is true:</span></span>

  - <span data-ttu-id="7b064-119">Ett nyckelord från Keyword_cc_verification hittas.</span><span class="sxs-lookup"><span data-stu-id="7b064-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="7b064-120">Ett nyckelord från Keyword_cc_name hittas</span><span class="sxs-lookup"><span data-stu-id="7b064-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="7b064-121">Funktionen Func_expiration_date hittar ett datum i rätt datumformat.</span><span class="sxs-lookup"><span data-stu-id="7b064-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="7b064-122">Kontrollsumman passerar</span><span class="sxs-lookup"><span data-stu-id="7b064-122">The checksum passes</span></span>

    <span data-ttu-id="7b064-123">Följande exempel skulle till exempel utlösa för en DLP-kreditkortsnummerpolicy:</span><span class="sxs-lookup"><span data-stu-id="7b064-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="7b064-124">Visum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="7b064-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="7b064-125">Löper ut: 2/2009</span><span class="sxs-lookup"><span data-stu-id="7b064-125">Expires: 2/2009</span></span>

<span data-ttu-id="7b064-126">Mer information om vad som krävs för att ett **kreditkortsnummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter kreditkort#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="7b064-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="7b064-127">Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="7b064-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  