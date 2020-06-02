---
title: DLP-regeln för amerikanskt/brittiskt passnummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507316"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="161c5-102">Problem med DLP - USA / Storbritannien passnummer</span><span class="sxs-lookup"><span data-stu-id="161c5-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="161c5-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="161c5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="161c5-104">**DLP-problem med passnummer mellan USA och Storbritannien**</span><span class="sxs-lookup"><span data-stu-id="161c5-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="161c5-105">Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett **passnummer** mellan USA och Storbritannien när du använder en DLP-känslig informationstyp i O365?</span><span class="sxs-lookup"><span data-stu-id="161c5-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="161c5-106">Om så är fallet, se till att ditt innehåll innehåller den information som behövs för vad DLP-principen letar efter när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="161c5-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="161c5-107">För en princip för passnummer i **USA/Storbritannien** som konfigurerats med en konfidensnivå på 75 %, utvärderas följande och måste identifieras för att regeln ska utlösas</span><span class="sxs-lookup"><span data-stu-id="161c5-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="161c5-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nio siffror</span><span class="sxs-lookup"><span data-stu-id="161c5-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="161c5-109">**[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nio på varandra följande siffror</span><span class="sxs-lookup"><span data-stu-id="161c5-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="161c5-110">**[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, det finns ingen Kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="161c5-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="161c5-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-princip är 75 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="161c5-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="161c5-112">Funktionen Func_usa_uk_passport hittar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="161c5-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="161c5-113">Ett nyckelord från Keyword_passport hittas.</span><span class="sxs-lookup"><span data-stu-id="161c5-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="161c5-114">Följande exempel skulle till exempel utlösa för **usa/brittisk passnummerpolicy:** U.S. Passport nummer 123456789</span><span class="sxs-lookup"><span data-stu-id="161c5-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="161c5-115">Mer information om vad som krävs för att ett passnummer i USA/Storbritannien ska upptäckas för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter amerikanskt/brittiskt passnummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="161c5-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="161c5-116">Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="161c5-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  