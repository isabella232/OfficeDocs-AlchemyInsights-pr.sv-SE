---
title: Tillträdestjänster pensionering
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747803"
---
# <a name="access-services-retirement"></a><span data-ttu-id="096e4-102">Tillträdestjänster pensionering</span><span class="sxs-lookup"><span data-stu-id="096e4-102">Access services retirement</span></span>

<span data-ttu-id="096e4-103">Som vi ursprungligen meddelade i MC97576, i mars 2017, och fortsatte att kommunicera under det gångna året tillgång tjänster håller på att dras tillbaka från Office 365.</span><span class="sxs-lookup"><span data-stu-id="096e4-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="096e4-104">Nästa fas i den här processen kommer att ta bort Access Web-databaser som använder SharePoint-listor som underliggande datalagring.</span><span class="sxs-lookup"><span data-stu-id="096e4-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="096e4-105">**Hur påverkar detta mig?**</span><span class="sxs-lookup"><span data-stu-id="096e4-105">**How does this affect me?**</span></span>

<span data-ttu-id="096e4-106">Från och med 2019 juni kommer vi att stoppa skapandet av nya Access-databaser i SharePoint Online och stänga av tjänsten och eventuella återstående appar i april 2020.</span><span class="sxs-lookup"><span data-stu-id="096e4-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="096e4-107">**Vad behöver jag göra för att förbereda mig för den här ändringen?**</span><span class="sxs-lookup"><span data-stu-id="096e4-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="096e4-108">Vi uppmuntrar dig att skapa en övergångsplan för organisationens Access-webbdatabaser.</span><span class="sxs-lookup"><span data-stu-id="096e4-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="096e4-109">Administratörer kan använda [appskannern för SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) för att få en inventering av de Access-appar som webbplatser använder.</span><span class="sxs-lookup"><span data-stu-id="096e4-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="096e4-110">Det finns flera sätt att migrera data för Access Web-databaser:</span><span class="sxs-lookup"><span data-stu-id="096e4-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="096e4-111">Importera till en lokal Access-databas (. ACCDB) eller till en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="096e4-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="096e4-112">Vi rekommenderar också att du utforskar Microsoft PowerApps som en alternativ plattform för att skapa affärslösningar utan kod för webb-och mobilenheter.</span><span class="sxs-lookup"><span data-stu-id="096e4-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>