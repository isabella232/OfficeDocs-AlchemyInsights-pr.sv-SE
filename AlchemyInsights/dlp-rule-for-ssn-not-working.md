---
title: DLP-regel för SSN fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389451"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="62fe4-102">DLP-problem med personnummer</span><span class="sxs-lookup"><span data-stu-id="62fe4-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="62fe4-103">Har du problem med **Data förlust Prevention (DLP)** fungerar inte för innehåll som innehåller **Social Security Number (SSN))** när du använder en typ av känslig information i Office 365?</span><span class="sxs-lookup"><span data-stu-id="62fe4-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="62fe4-104">Om så är fallet, kontrollera innehållet innehåller informationen som krävs för vad DLP-princip söker.</span><span class="sxs-lookup"><span data-stu-id="62fe4-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="62fe4-105">Till exempel för en SSN-princip som konfigurerats med en konfidensnivå på 85% följande utvärderas och måste identifieras att utlösa regeln:</span><span class="sxs-lookup"><span data-stu-id="62fe4-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="62fe4-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 siffror, som kan vara i en formaterad eller oformaterad mönster</span><span class="sxs-lookup"><span data-stu-id="62fe4-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="62fe4-107">**[Mönster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fyra funktioner är SSNs i fyra olika mönster:</span><span class="sxs-lookup"><span data-stu-id="62fe4-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="62fe4-108">Func_ssn hittas SSNs med pre-2011 starka formatering som är formaterade med streck och blanksteg (ddd-dd-dddd eller ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="62fe4-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="62fe4-109">Func_unformatted_ssn hittas SSNs med pre-2011 starka formatering som är oformaterad som nio på varandra följande siffror (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="62fe4-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="62fe4-110">Func_randomized_formatted_ssn söker efter inlägg 2011-SSNs som är formaterade med streck och blanksteg (ddd-dd-dddd eller ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="62fe4-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="62fe4-111">Func_randomized_unformatted_ssn söker efter inlägg 2011-SSNs som är oformaterad som nio på varandra följande siffror (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="62fe4-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="62fe4-112">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, det finns ingen kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="62fe4-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="62fe4-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-princip är 85% säker på att den har upptäckt att den här typen av känslig information om inom ett avstånd av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="62fe4-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="62fe4-114">[Funktionen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) returnerar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="62fe4-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="62fe4-115">Det finns ett nyckelord från [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="62fe4-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="62fe4-116">Innehåller exempel på nyckelord: *Social trygghet, Social trygghet #, Soc sek, SSN* .</span><span class="sxs-lookup"><span data-stu-id="62fe4-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="62fe4-117">Till exempel i följande exempel initierar för principen DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="62fe4-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="62fe4-118">Mer information om vad som krävs för SSNs ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad den känsliga informationstyper leta efter SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="62fe4-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="62fe4-119">Med en annan inbyggd känslig information-typ finns i följande artikel för information om vad som krävs för andra typer: [vad den känsliga informationstyper leta efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="62fe4-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  