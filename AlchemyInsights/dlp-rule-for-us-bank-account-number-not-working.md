---
title: DLP-regel för amerikanskt bankkontonummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704057"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="a7e60-102">DLP-problem med amerikanska bankkontonummer</span><span class="sxs-lookup"><span data-stu-id="a7e60-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="a7e60-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a7e60-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a7e60-104">**DLP-problem med amerikanska bankkontonummer**</span><span class="sxs-lookup"><span data-stu-id="a7e60-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="a7e60-105">Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett amerikanskt **bankkontonummer** när du använder en DLP-känslig informationstyp i O365?</span><span class="sxs-lookup"><span data-stu-id="a7e60-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a7e60-106">Om så är fallet, se till att ditt innehåll innehåller den information som behövs för vad DLP-principen letar efter när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="a7e60-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="a7e60-107">För en princip för **amerikanskt bankkontonummer** som konfigurerats med en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:</span><span class="sxs-lookup"><span data-stu-id="a7e60-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a7e60-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 siffror</span><span class="sxs-lookup"><span data-stu-id="a7e60-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="a7e60-109">**[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 på varandra följande siffror.</span><span class="sxs-lookup"><span data-stu-id="a7e60-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="a7e60-110">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, det finns ingen Kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="a7e60-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="a7e60-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** En DLP-princip är 75 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="a7e60-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a7e60-112">Det reguljära uttrycket Regex_usa_bank_account_number hittar innehåll som matchar mönstret</span><span class="sxs-lookup"><span data-stu-id="a7e60-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="a7e60-113">Ett nyckelord från Keyword_usa_Bank_Account hittas.</span><span class="sxs-lookup"><span data-stu-id="a7e60-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="a7e60-114">Följande exempel skulle till exempel utlösa för policyn för **amerikanskt bankkontonummer:** Checkkonto 78344011</span><span class="sxs-lookup"><span data-stu-id="a7e60-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="a7e60-115">Mer information om vad som krävs för att ett **amerikanskt bankkontonummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter amerikanskt bankkontonummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="a7e60-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="a7e60-116">Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a7e60-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  