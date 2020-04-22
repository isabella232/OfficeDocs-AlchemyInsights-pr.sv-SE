---
title: Tillgång till tjänster pensionering
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687276"
---
# <a name="access-services-retirement"></a><span data-ttu-id="b8262-102">Tillgång till tjänster pensionering</span><span class="sxs-lookup"><span data-stu-id="b8262-102">Access services retirement</span></span>

<span data-ttu-id="b8262-103">Som vi ursprungligen tillkännagav i MC97576, i mars 2017, och fortsatte att kommunicera under det senaste året access services dras tillbaka.</span><span class="sxs-lookup"><span data-stu-id="b8262-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="b8262-104">Nästa fas i den här processen blir borttagningen av Access-webbdatabaser som använder SharePoint-listor som underliggande datalagring.</span><span class="sxs-lookup"><span data-stu-id="b8262-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="b8262-105">**Hur påverkar detta mig?**</span><span class="sxs-lookup"><span data-stu-id="b8262-105">**How does this affect me?**</span></span>

<span data-ttu-id="b8262-106">Från och med juni 2019 kommer vi att sluta skapa nya Access-databaser i SharePoint Online och stänga av tjänsten och eventuella återstående appar senast i april 2020.</span><span class="sxs-lookup"><span data-stu-id="b8262-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="b8262-107">**Vad behöver jag göra för att förbereda mig för den här ändringen?**</span><span class="sxs-lookup"><span data-stu-id="b8262-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="b8262-108">Vi rekommenderar att du skapar en övergångsplan för organisationens Access-webbdatabaser.</span><span class="sxs-lookup"><span data-stu-id="b8262-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="b8262-109">Administratörer kan använda [SharePoint Access-appskannern](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) för att få en inventering av Access-apparna som webbplatserna använder.</span><span class="sxs-lookup"><span data-stu-id="b8262-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="b8262-110">Det finns flera sätt att migrera Data i Access-webbdatabaser:</span><span class="sxs-lookup"><span data-stu-id="b8262-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="b8262-111">Importera till en lokal Access-databas (. ACCDB) eller till en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="b8262-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="b8262-112">Vi rekommenderar också att du utforskar Microsoft PowerApps som en alternativ plattform för att skapa lösningar utan kod för webb- och mobila enheter.</span><span class="sxs-lookup"><span data-stu-id="b8262-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>