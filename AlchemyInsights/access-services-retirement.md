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
# <a name="access-services-retirement"></a>Access services-pension

Som vi ursprungligen angivits i MC97576, i mars 2017 och fortsatte att kommunicera under det senaste året är tjänster som dras tillbaka från Office 365. Nästa fas i processen kommer att borttagningen av Access Web-databaser som använder SharePoint-listor som deras underliggande datalagring.

## <a name="how-does-this-affect-me"></a>Hur påverkar det här mig?

Från juni 2019 kan vi avbryta skapandet av nya Access-databaser i SharePoint Online och avsluta tjänsten och eventuella återstående apps April 2020.

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a>Vad behöver jag göra för att förbereda för den här ändringen?

Vi rekommenderar att du skapar en plan för övergång för organisationens Access web-databaser. Administratörer kan använda [skanner för åtkomst till SharePoint-app](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) för att hämta en inventering av Access apps webbplatser använder. 

Det finns flera sätt att migrera data för Access web-databaser:

- Importera lokala Access-databaser (. ACCDB) eller till en Excelfil.
- Vi rekommenderar också att utforska Microsoft PowerApps som en alternativ plattform för att skapa affärslösningar med ingen kod för webben och mobila enheter.