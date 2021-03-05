---
title: Om Exchange Server säkerhetsuppdateringar
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482986"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="b3e4a-102">Om Exchange Server säkerhetsuppdateringar</span><span class="sxs-lookup"><span data-stu-id="b3e4a-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="b3e4a-103">Microsoft har släppt en serie kritiska säkerhetsuppdateringar för Exchange Server lokalt.</span><span class="sxs-lookup"><span data-stu-id="b3e4a-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="b3e4a-104">De aktuella serverversionerna är uppdateringsnivåer för Exchange Server 2010, 2013, 2016 och 2019.</span><span class="sxs-lookup"><span data-stu-id="b3e4a-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="b3e4a-105">Exchange Online påverkas INTE, men om du har några lokala Exchange-servrar på grund av hybridkonfigurationen är de potentiellt sårbara.</span><span class="sxs-lookup"><span data-stu-id="b3e4a-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="b3e4a-106">Om du vill uppdatera dina lokala servrar måste du köra minst följande versioner av Exchange:</span><span class="sxs-lookup"><span data-stu-id="b3e4a-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="b3e4a-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="b3e4a-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="b3e4a-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="b3e4a-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="b3e4a-109">Exchange Server 2016 CU 19 eller CU 18</span><span class="sxs-lookup"><span data-stu-id="b3e4a-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="b3e4a-110">Exchange Server 2019 CU 8 eller CU 7</span><span class="sxs-lookup"><span data-stu-id="b3e4a-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="b3e4a-111">Se följande meddelande om placeringen av korrigeringar: [släpptes: mars 2021 Exchange Server säkerhetsuppdateringar](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="b3e4a-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="b3e4a-112">**Viktiga kommentarer:**</span><span class="sxs-lookup"><span data-stu-id="b3e4a-112">**Important notes:**</span></span>

<span data-ttu-id="b3e4a-113">Installation av uppdateringar fungerar inte om dina lokala servrar inte kör nödvändiga Exchange-versioner, enligt ovanstående lista.</span><span class="sxs-lookup"><span data-stu-id="b3e4a-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="b3e4a-114">Om du installerar uppdateringar manuellt läser du avsnittet "Kända problem" i KB-uppdateringsartiklarna för viktig information.</span><span class="sxs-lookup"><span data-stu-id="b3e4a-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="b3e4a-115">Säkerhetsuppdateringar MÅSTE köras från cmd/PowerShell-uppmaningen för förhöjda cmd!</span><span class="sxs-lookup"><span data-stu-id="b3e4a-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
