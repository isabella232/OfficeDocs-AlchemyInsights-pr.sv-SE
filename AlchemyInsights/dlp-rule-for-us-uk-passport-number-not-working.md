---
title: DLP-regeln för amerikanskt/brittiskt passnummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931280"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="d2fe7-102">Problem med DLP - USA / Storbritannien passnummer</span><span class="sxs-lookup"><span data-stu-id="d2fe7-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="d2fe7-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d2fe7-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d2fe7-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d2fe7-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d2fe7-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d2fe7-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d2fe7-109">**DLP-problem med passnummer mellan USA och Storbritannien**</span><span class="sxs-lookup"><span data-stu-id="d2fe7-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="d2fe7-110">Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett **passnummer** mellan USA och Storbritannien när du använder en DLP-känslig informationstyp i O365?</span><span class="sxs-lookup"><span data-stu-id="d2fe7-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="d2fe7-111">Om så är fallet, se till att ditt innehåll innehåller den information som behövs för vad DLP-principen letar efter när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="d2fe7-112">För en princip för passnummer i **USA/Storbritannien** som konfigurerats med en konfidensnivå på 75 %, utvärderas följande och måste identifieras för att regeln ska utlösas</span><span class="sxs-lookup"><span data-stu-id="d2fe7-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="d2fe7-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nio siffror</span><span class="sxs-lookup"><span data-stu-id="d2fe7-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="d2fe7-114">**[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nio på varandra följande siffror</span><span class="sxs-lookup"><span data-stu-id="d2fe7-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="d2fe7-115">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, det finns ingen Kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="d2fe7-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="d2fe7-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** En DLP-princip är 75 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="d2fe7-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="d2fe7-117">Funktionen Func_usa_uk_passport hittar innehåll som matchar mönstret.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="d2fe7-118">Ett nyckelord från Keyword_passport hittas.</span><span class="sxs-lookup"><span data-stu-id="d2fe7-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="d2fe7-119">Följande exempel skulle till exempel utlösa för **usa/brittisk passnummerpolicy:** U.S. Passport nummer 123456789</span><span class="sxs-lookup"><span data-stu-id="d2fe7-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="d2fe7-120">Mer information om vad som krävs för att ett passnummer i USA/Storbritannien ska upptäckas för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter amerikanskt/brittiskt passnummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="d2fe7-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="d2fe7-121">Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d2fe7-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  