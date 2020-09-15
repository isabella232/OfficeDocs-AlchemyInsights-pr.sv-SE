---
title: DLP-regel för SSN fungerar inte
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679387"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="a9833-102">DLP-problem med person nummer</span><span class="sxs-lookup"><span data-stu-id="a9833-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="a9833-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a9833-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a9833-104">**DLP-problem med efter SSN efter**</span><span class="sxs-lookup"><span data-stu-id="a9833-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="a9833-105">Har du problem med **data förlust skydd (DLP)** fungerar inte för innehåll som innehåller ett **person nummer (SSN)** när du använder en känslig informations typ i Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="a9833-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="a9833-106">Om så är fallet kontrollerar du att innehållet innehåller den information som behövs för att använda DLP-policyn.</span><span class="sxs-lookup"><span data-stu-id="a9833-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="a9833-107">För exempelvis en SSN-princip som har kon figurer ATS med en konfidensnivå på 85% utvärderas följande och måste identifieras för att regeln ska utlösa:</span><span class="sxs-lookup"><span data-stu-id="a9833-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a9833-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 siffror, som kan vara i ett formaterat eller oformaterat mönster</span><span class="sxs-lookup"><span data-stu-id="a9833-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="a9833-109">**[Mönster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fyra funktioner letar efter efter SSN efter i fyra olika mönster:</span><span class="sxs-lookup"><span data-stu-id="a9833-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="a9833-110">Func_ssn hittar efter SSN efter med för2011 stark formatering som formaterats med tank streck eller blank steg (DDD-DD-dddd eller DDD mm dddd)</span><span class="sxs-lookup"><span data-stu-id="a9833-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="a9833-111">Func_unformatted_ssn hittar efter SSN efter med förformaterad formatering som är oformaterad 2011 med nio efterföljande siffror (sssssssss)</span><span class="sxs-lookup"><span data-stu-id="a9833-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="a9833-112">Func_randomized_formatted_ssn hittar inlägg-2011-efter SSN efter som formaterats med tank streck eller blank steg (DDD-DD-dddd eller DDD mm dddd)</span><span class="sxs-lookup"><span data-stu-id="a9833-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="a9833-113">Func_randomized_unformatted_ssn hittar efter-2011-efter SSN efter som är oformaterade med nio efterföljande siffror (sssssssss)</span><span class="sxs-lookup"><span data-stu-id="a9833-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="a9833-114">**[Kontroll Summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nej, det finns ingen kontroll Summa</span><span class="sxs-lookup"><span data-stu-id="a9833-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="a9833-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-princip är 85% trygg att den här typen av känslig information identifieras om, inom ett avstånd på 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="a9833-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a9833-116">[Funktionen Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) hittar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="a9833-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a9833-117">Ett nyckelord från [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) hittas.</span><span class="sxs-lookup"><span data-stu-id="a9833-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="a9833-118">Exempel på nyckelord:  *social trygghet, social trygghet #, SOC SEK, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="a9833-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="a9833-119">Följande exempel skulle till exempel utlösas för policyn DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="a9833-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="a9833-120">Mer information om vad som krävs för att efter SSN efter ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [vad den känsliga informations typen letar efter efter SSN efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="a9833-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="a9833-121">Om du använder en annan inbyggd känslig informations typ kan du läsa följande artikel för information om vad som är obligatoriskt för andra typer: [vad den känsliga informations typen letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="a9833-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  