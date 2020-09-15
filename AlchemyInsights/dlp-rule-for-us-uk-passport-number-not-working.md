---
title: DLP-regel för AMERIKANSKt/brittiska Passport-nummer fungerar inte
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679242"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="d1a2b-102">Problem med DLP-amerikanska/brittiska Passport-nummer</span><span class="sxs-lookup"><span data-stu-id="d1a2b-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="d1a2b-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="d1a2b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d1a2b-104">**DLP-problem med amerikanska/brittiska Passport-nummer**</span><span class="sxs-lookup"><span data-stu-id="d1a2b-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="d1a2b-105">Har du problem med **data förlust skydd (DLP)** fungerar inte för innehåll som innehåller ett **USA/UK Passport-nummer** när du använder en DLP-känslig informations typ i O365?</span><span class="sxs-lookup"><span data-stu-id="d1a2b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d1a2b-106">I så fall bör du kontrol lera att innehållet innehåller den information som behövs för att DLP-policyn ska identifieras när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="d1a2b-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d1a2b-107">För att en policy för principer för ett **svenskt och brittiskt nummer** som har kon figurer ATS med en konfidensnivå på 75% utvärderas till exempel följande och måste identifieras för att regeln ska utlösa</span><span class="sxs-lookup"><span data-stu-id="d1a2b-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="d1a2b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nio siffror</span><span class="sxs-lookup"><span data-stu-id="d1a2b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="d1a2b-109">**[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nio siffror i följd</span><span class="sxs-lookup"><span data-stu-id="d1a2b-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="d1a2b-110">**[Kontroll Summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, det finns ingen kontroll Summa</span><span class="sxs-lookup"><span data-stu-id="d1a2b-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d1a2b-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-princip är 75% trygg att den här typen av känslig information identifieras om, inom ett avstånd på 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="d1a2b-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d1a2b-112">Funktionen Func_usa_uk_passport hittar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="d1a2b-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d1a2b-113">Ett nyckelord från Keyword_passport hittas.</span><span class="sxs-lookup"><span data-stu-id="d1a2b-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="d1a2b-114">Följande exempel skulle till exempel utlösas för policyn **amerikanska/brittiska pass nummer** : U.S. passport Number 123456789</span><span class="sxs-lookup"><span data-stu-id="d1a2b-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="d1a2b-115">Mer information om vad som krävs för att ett SVENSKt och brittiska Passport-nummer ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [vad den känsliga informations typen letar efter USA/brittiska pass nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="d1a2b-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="d1a2b-116">Om du använder en annan inbyggd känslig informations typ kan du läsa följande artikel för information om vad som är obligatoriskt för andra typer: [vad den känsliga informations typen letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d1a2b-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  