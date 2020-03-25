---
title: DLP-regel för amerikanskt bankkontonummer fungerar inte
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
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932568"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="a2681-102">DLP-problem med amerikanska bankkontonummer</span><span class="sxs-lookup"><span data-stu-id="a2681-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="a2681-103">**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden.</span><span class="sxs-lookup"><span data-stu-id="a2681-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a2681-104">Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar.</span><span class="sxs-lookup"><span data-stu-id="a2681-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a2681-105">Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.</span><span class="sxs-lookup"><span data-stu-id="a2681-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a2681-106">Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid.</span><span class="sxs-lookup"><span data-stu-id="a2681-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a2681-107">Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider.</span><span class="sxs-lookup"><span data-stu-id="a2681-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a2681-108">Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.</span><span class="sxs-lookup"><span data-stu-id="a2681-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a2681-109">**DLP-problem med amerikanska bankkontonummer**</span><span class="sxs-lookup"><span data-stu-id="a2681-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="a2681-110">Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett amerikanskt **bankkontonummer** när du använder en DLP-känslig informationstyp i O365?</span><span class="sxs-lookup"><span data-stu-id="a2681-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a2681-111">Om så är fallet, se till att ditt innehåll innehåller den information som behövs för vad DLP-principen letar efter när den utvärderas.</span><span class="sxs-lookup"><span data-stu-id="a2681-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="a2681-112">För en princip för **amerikanskt bankkontonummer** som konfigurerats med en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:</span><span class="sxs-lookup"><span data-stu-id="a2681-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a2681-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 siffror</span><span class="sxs-lookup"><span data-stu-id="a2681-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="a2681-114">**[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 på varandra följande siffror.</span><span class="sxs-lookup"><span data-stu-id="a2681-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="a2681-115">**[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, det finns ingen Kontrollsumma</span><span class="sxs-lookup"><span data-stu-id="a2681-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="a2681-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** En DLP-princip är 75 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:</span><span class="sxs-lookup"><span data-stu-id="a2681-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a2681-117">Det reguljära uttrycket Regex_usa_bank_account_number hittar innehåll som matchar mönstret</span><span class="sxs-lookup"><span data-stu-id="a2681-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="a2681-118">Ett nyckelord från Keyword_usa_Bank_Account hittas.</span><span class="sxs-lookup"><span data-stu-id="a2681-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="a2681-119">Följande exempel skulle till exempel utlösa för policyn för **amerikanskt bankkontonummer:** Checkkonto 78344011</span><span class="sxs-lookup"><span data-stu-id="a2681-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="a2681-120">Mer information om vad som krävs för att ett **amerikanskt bankkontonummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter amerikanskt bankkontonummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="a2681-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="a2681-121">Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="a2681-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  