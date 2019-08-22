---
title: DLP-regel för oss bankkontonummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529901"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="d134c-102">DLP-problem med oss bankkontonummer</span><span class="sxs-lookup"><span data-stu-id="d134c-102">DLP issues with US Bank Account Numbers</span></span>

<span data-ttu-id="d134c-103">Har du problem med **Data förlust Prevention (DLP)** fungerar inte för innehåll som innehåller ett **Bankkontonummer för USA** när du använder en DLP känslig informationstyp i O365?</span><span class="sxs-lookup"><span data-stu-id="d134c-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d134c-104">Om så är fallet kontrollerar du att ditt innehåll innehåller informationen som krävs för vilka principen DLP söker efter när det utvärderas.</span><span class="sxs-lookup"><span data-stu-id="d134c-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d134c-105">Till exempel för en **Amerikansk bankkontonummer** princip som konfigurerats med en konfidensnivå på 85% följande utvärderas och måste identifieras att utlösa regeln:</span><span class="sxs-lookup"><span data-stu-id="d134c-105">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="d134c-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 siffror</span><span class="sxs-lookup"><span data-stu-id="d134c-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="d134c-107">**[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 på varandra följande siffror.</span><span class="sxs-lookup"><span data-stu-id="d134c-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="d134c-108">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, det finns ingen kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="d134c-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d134c-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** En DLP-princip är 75% säker på att den har upptäckt att den här typen av känslig information om inom ett avstånd av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="d134c-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d134c-110">Hittar innehåll som matchar mönstret för det reguljära uttrycket Regex_usa_bank_account_number</span><span class="sxs-lookup"><span data-stu-id="d134c-110">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="d134c-111">Det finns ett nyckelord från Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="d134c-111">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="d134c-112">Till exempel i följande exempel initierar principens **Amerikanska bankkontonummer** : checkkonto 78344011</span><span class="sxs-lookup"><span data-stu-id="d134c-112">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="d134c-113">Mer information om vad som krävs för **USA bankkontonumret** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad den känsliga informationstyper leta efter amerikanska bankkontonummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="d134c-113">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="d134c-114">Med en annan inbyggd känslig information-typ finns i följande artikel för information om vad som krävs för andra typer: [vad den känsliga informationstyper leta efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d134c-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  