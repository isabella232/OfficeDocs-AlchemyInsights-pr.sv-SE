---
title: Dragning av Access Services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698700"
---
# <a name="access-services-retirement"></a><span data-ttu-id="60e47-102">Dragning av Access Services</span><span class="sxs-lookup"><span data-stu-id="60e47-102">Access services retirement</span></span>

<span data-ttu-id="60e47-103">Som vi presenterade ursprungligen annonserade i MC97576 mars 2017 och fortsatte att kommunicera under det tidigare året Access Services håller på att avvecklas.</span><span class="sxs-lookup"><span data-stu-id="60e47-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="60e47-104">Nästa steg i processen kommer att ta bort Access-webbdatabaser som använder SharePoint-listor som sin underliggande data lagring.</span><span class="sxs-lookup"><span data-stu-id="60e47-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="60e47-105">**Hur påverkar detta mig?**</span><span class="sxs-lookup"><span data-stu-id="60e47-105">**How does this affect me?**</span></span>

<span data-ttu-id="60e47-106">Från och med den 2019 juni kommer vi att sluta skapa nya Access-databaser i SharePoint Online och stänga av tjänsten och eventuella återstående appar från april 2020.</span><span class="sxs-lookup"><span data-stu-id="60e47-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="60e47-107">**Vad behöver jag göra för att förbereda den här ändringen?**</span><span class="sxs-lookup"><span data-stu-id="60e47-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="60e47-108">Vi uppmuntrar dig att skapa ett över gångs abonnemang för organisationens Access-webbdatabaser.</span><span class="sxs-lookup"><span data-stu-id="60e47-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="60e47-109">Administratörer kan använda [program skannern för SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) för att få en inventering av de Access-appar som webbplatser använder.</span><span class="sxs-lookup"><span data-stu-id="60e47-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="60e47-110">Det finns flera sätt att migrera webb databas data från Access:</span><span class="sxs-lookup"><span data-stu-id="60e47-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="60e47-111">Importera till en lokal Access-databas (. ACCDB) eller till en Excel-fil.</span><span class="sxs-lookup"><span data-stu-id="60e47-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="60e47-112">Vi rekommenderar också att du utforskar Microsoft PowerApps som en alternativ plattform för att skapa företags lösningar utan kod för webb-och mobila enheter.</span><span class="sxs-lookup"><span data-stu-id="60e47-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>