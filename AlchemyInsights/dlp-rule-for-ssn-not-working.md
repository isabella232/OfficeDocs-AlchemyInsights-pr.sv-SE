---
title: DLP-regeln för SSN fungerar inte
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
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977324"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="62124-102">DLP-problem med personnummer</span><span class="sxs-lookup"><span data-stu-id="62124-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="62124-103">**Viktigt:** Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga – Besök [Tillfälliga funktionsjusteringar](https://aka.ms/ODSPAdjustments) för SharePoint Online för mer information.</span><span class="sxs-lookup"><span data-stu-id="62124-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="62124-104">**DLP-problem med SSN-nätverk**</span><span class="sxs-lookup"><span data-stu-id="62124-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="62124-105">Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett **personnummer (SSN)** när du använder en känslig informationstyp i Office 365?</span><span class="sxs-lookup"><span data-stu-id="62124-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="62124-106">Om så är fallet, se till att ditt innehåll innehåller den information som behövs för vad DLP-principen söker.</span><span class="sxs-lookup"><span data-stu-id="62124-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="62124-107">För en SSN-princip som konfigurerats med en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:</span><span class="sxs-lookup"><span data-stu-id="62124-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="62124-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 siffror, som kan vara i ett formaterat eller oformaterat mönster</span><span class="sxs-lookup"><span data-stu-id="62124-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="62124-109">**[Mönster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fyra funktioner letar efter SSN i fyra olika mönster:</span><span class="sxs-lookup"><span data-stu-id="62124-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="62124-110">Func_ssn hittar SSN med stark formatering före 2011 som är formaterad med streck eller blanksteg (ddd-ddd-dddd ELLER ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="62124-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="62124-111">Func_unformatted_ssn hittar SSN med stark formatering före 2011 som är oformaterade som nio på varandra följande siffror (ddddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="62124-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="62124-112">Func_randomized_formatted_ssn hittar SSN efter 2011 som är formaterade med streck eller blanksteg (ddd-dddd ELLER ddd ddd ddddd)</span><span class="sxs-lookup"><span data-stu-id="62124-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="62124-113">Func_randomized_unformatted_ssn hittar SSN efter 2011 som är oformaterade som nio på varandra följande siffror (dddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="62124-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="62124-114">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, det finns ingen Kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="62124-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="62124-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-princip är 85 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="62124-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="62124-116">[Funktionen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) hittar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="62124-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="62124-117">Ett nyckelord från [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) hittas.</span><span class="sxs-lookup"><span data-stu-id="62124-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="62124-118">Exempel på nyckelord är: *Social Security, Social Security #, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="62124-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="62124-119">Följande exempel skulle till exempel utlösa för DLP SSN-principen: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="62124-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="62124-120">Mer information om vad som krävs för att SSN ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter SSN-nätverk](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="62124-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="62124-121">Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="62124-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  