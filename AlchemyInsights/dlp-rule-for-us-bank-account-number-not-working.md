---
title: DLP-regel för AMERIKANSKt bankkonto nummer fungerar inte
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679314"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="74c3c-102">DLP-problem med amerikanska bank konto nummer</span><span class="sxs-lookup"><span data-stu-id="74c3c-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="74c3c-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="74c3c-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="74c3c-104">**DLP-problem med amerikanska bank konto nummer**</span><span class="sxs-lookup"><span data-stu-id="74c3c-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="74c3c-105">Har du problem med **data förlust skydd (DLP)** fungerar inte för innehåll som innehåller ett **amerikanskt bankkonto nummer** när du använder en typ av DLP-känslig information i O365?</span><span class="sxs-lookup"><span data-stu-id="74c3c-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="74c3c-106">I så fall bör du kontrol lera att innehållet innehåller den information som behövs för att DLP-policyn ska identifieras när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="74c3c-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="74c3c-107">Om till exempel en policy för **amerikansk bank konto nummer** har kon figurer ATS med en konfidensnivå på 85% utvärderas följande och måste identifieras för att regeln ska utlösa:</span><span class="sxs-lookup"><span data-stu-id="74c3c-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="74c3c-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 siffror</span><span class="sxs-lookup"><span data-stu-id="74c3c-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="74c3c-109">**[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 siffror i följd.</span><span class="sxs-lookup"><span data-stu-id="74c3c-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="74c3c-110">**[Kontroll Summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, det finns ingen kontroll Summa</span><span class="sxs-lookup"><span data-stu-id="74c3c-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="74c3c-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-princip är 75% trygg att den här typen av känslig information identifieras om, inom ett avstånd på 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="74c3c-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="74c3c-112">Det reguljära uttrycket Regex_usa_bank_account_number hittar innehåll som matchar mönstret</span><span class="sxs-lookup"><span data-stu-id="74c3c-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="74c3c-113">Ett nyckelord från Keyword_usa_Bank_Account hittas.</span><span class="sxs-lookup"><span data-stu-id="74c3c-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="74c3c-114">Följande exempel skulle till exempel utlösa policyn för **bank konto nummer för USA** för att kontrol lera konto 78344011</span><span class="sxs-lookup"><span data-stu-id="74c3c-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="74c3c-115">Mer information om vad som krävs för att ett **amerikanskt bank konto nummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [vad de känsliga informations typerna ser ut för ditt bank konto nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="74c3c-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="74c3c-116">Om du använder en annan inbyggd känslig informations typ kan du läsa följande artikel för information om vad som är obligatoriskt för andra typer: [vad den känsliga informations typen letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="74c3c-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  