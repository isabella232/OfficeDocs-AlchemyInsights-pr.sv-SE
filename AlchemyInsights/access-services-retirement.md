---
title: Access services-pension
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973954"
---
# <a name="access-services-retirement"></a><span data-ttu-id="44119-102">Access services-pension</span><span class="sxs-lookup"><span data-stu-id="44119-102">Access services retirement</span></span>

<span data-ttu-id="44119-103">Som vi ursprungligen angivits i MC97576, i mars 2017 och fortsatte att kommunicera under det senaste året är tjänster som dras tillbaka från Office 365.</span><span class="sxs-lookup"><span data-stu-id="44119-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="44119-104">Nästa fas i processen kommer att borttagningen av Access Web-databaser som använder SharePoint-listor som deras underliggande datalagring.</span><span class="sxs-lookup"><span data-stu-id="44119-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="44119-105">Hur påverkar det här mig?</span><span class="sxs-lookup"><span data-stu-id="44119-105">How does this affect me?</span></span>

<span data-ttu-id="44119-106">Från juni 2019 kan vi avbryta skapandet av nya Access-databaser i SharePoint Online och avsluta tjänsten och eventuella återstående apps April 2020.</span><span class="sxs-lookup"><span data-stu-id="44119-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="44119-107">Vad behöver jag göra för att förbereda för den här ändringen?</span><span class="sxs-lookup"><span data-stu-id="44119-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="44119-108">Vi rekommenderar att du skapar en plan för övergång för organisationens Access web-databaser.</span><span class="sxs-lookup"><span data-stu-id="44119-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="44119-109">Administratörer kan använda [skanner för åtkomst till SharePoint-app](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) för att hämta en inventering av Access apps webbplatser använder.</span><span class="sxs-lookup"><span data-stu-id="44119-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="44119-110">Det finns flera sätt att migrera data för Access web-databaser:</span><span class="sxs-lookup"><span data-stu-id="44119-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="44119-111">Importera lokala Access-databaser (. ACCDB) eller till en Excelfil.</span><span class="sxs-lookup"><span data-stu-id="44119-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="44119-112">Vi rekommenderar också att utforska Microsoft PowerApps som en alternativ plattform för att skapa affärslösningar med ingen kod för webben och mobila enheter.</span><span class="sxs-lookup"><span data-stu-id="44119-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>