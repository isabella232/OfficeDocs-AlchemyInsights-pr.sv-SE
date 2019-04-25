---
title: DLP-regel för USA / Storbritannien passnummer fungerar inte
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404399"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="a1e9c-102">Problem med DLP - USA / Storbritannien Passport tal</span><span class="sxs-lookup"><span data-stu-id="a1e9c-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="a1e9c-103">Har du problem med **Data förlust Prevention (DLP)** fungerar inte för innehåll som innehåller en **US / UK passnummer** när du använder en DLP känslig informationstyp i O365?</span><span class="sxs-lookup"><span data-stu-id="a1e9c-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a1e9c-104">Om så är fallet kontrollerar du att ditt innehåll innehåller informationen som krävs för vilka principen DLP söker efter när det utvärderas.</span><span class="sxs-lookup"><span data-stu-id="a1e9c-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="a1e9c-105">Till exempel för en **US / UK passnummer** princip har konfigurerats med en konfidensnivå på 75%, följande utvärderas och måste identifieras för att regeln ska utlösa</span><span class="sxs-lookup"><span data-stu-id="a1e9c-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="a1e9c-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nio siffror</span><span class="sxs-lookup"><span data-stu-id="a1e9c-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="a1e9c-107">**[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nio på varandra följande siffror</span><span class="sxs-lookup"><span data-stu-id="a1e9c-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="a1e9c-108">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, det finns ingen kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="a1e9c-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="a1e9c-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** En DLP-princip är 75% säker på att den har upptäckt att den här typen av känslig information om inom ett avstånd av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="a1e9c-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="a1e9c-110">Funktionen Func_usa_uk_passport returnerar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="a1e9c-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="a1e9c-111">Det finns ett nyckelord från Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="a1e9c-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="a1e9c-112">Till exempel i följande exempel initierar för den **US / UK passnummer** princip: amerikanskt pass nummer 123456789</span><span class="sxs-lookup"><span data-stu-id="a1e9c-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="a1e9c-113">Mer information om vad som krävs för en USA eller Storbritannien passnummer ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [vad den känsliga informationstyper utseende för USA / Storbritannien passnummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="a1e9c-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="a1e9c-114">Med en annan inbyggd känslig information-typ finns i följande artikel för information om vad som krävs för andra typer: [vad den känsliga informationstyper leta efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a1e9c-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

