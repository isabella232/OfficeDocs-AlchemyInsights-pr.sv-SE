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
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932554"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="d58a0-102">DLP-problem med personnummer</span><span class="sxs-lookup"><span data-stu-id="d58a0-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="d58a0-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="d58a0-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d58a0-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="d58a0-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d58a0-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="d58a0-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d58a0-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="d58a0-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d58a0-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="d58a0-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d58a0-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="d58a0-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d58a0-109">**DLP-problem med SSN-nätverk**</span><span class="sxs-lookup"><span data-stu-id="d58a0-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="d58a0-110">Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett **personnummer (SSN)** när du använder en känslig informationstyp i Office 365?</span><span class="sxs-lookup"><span data-stu-id="d58a0-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="d58a0-111">Om så är fallet, se till att ditt innehåll innehåller den information som behövs för vad DLP-principen söker.</span><span class="sxs-lookup"><span data-stu-id="d58a0-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="d58a0-112">För en SSN-princip som konfigurerats med en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:</span><span class="sxs-lookup"><span data-stu-id="d58a0-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d58a0-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 siffror, som kan vara i ett formaterat eller oformaterat mönster</span><span class="sxs-lookup"><span data-stu-id="d58a0-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="d58a0-114">**[Mönster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fyra funktioner letar efter SSN i fyra olika mönster:</span><span class="sxs-lookup"><span data-stu-id="d58a0-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="d58a0-115">Func_ssn hittar SSN med stark formatering före 2011 som är formaterad med streck eller blanksteg (ddd-ddd-dddd ELLER ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="d58a0-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d58a0-116">Func_unformatted_ssn hittar SSN med stark formatering före 2011 som är oformaterade som nio på varandra följande siffror (ddddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="d58a0-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="d58a0-117">Func_randomized_formatted_ssn hittar SSN efter 2011 som är formaterade med streck eller blanksteg (ddd-dddd ELLER ddd ddd ddddd)</span><span class="sxs-lookup"><span data-stu-id="d58a0-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="d58a0-118">Func_randomized_unformatted_ssn hittar SSN efter 2011 som är oformaterade som nio på varandra följande siffror (dddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="d58a0-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="d58a0-119">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, det finns ingen Kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="d58a0-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="d58a0-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-princip är 85 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="d58a0-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d58a0-121">[Funktionen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) hittar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="d58a0-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d58a0-122">Ett nyckelord från [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) hittas.</span><span class="sxs-lookup"><span data-stu-id="d58a0-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="d58a0-123">Exempel på nyckelord är: *Social Security, Social Security #, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="d58a0-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="d58a0-124">Följande exempel skulle till exempel utlösa för DLP SSN-principen: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="d58a0-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="d58a0-125">Mer information om vad som krävs för att SSN ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter SSN-nätverk](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="d58a0-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="d58a0-126">Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d58a0-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  