---
title: Access services-pension
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495769"
---
# <a name="access-services-retirement"></a>Access services-pension

Som vi ursprungligen angivits i MC97576, i mars 2017 och fortsatte att kommunicera under det senaste året är tjänster som dras tillbaka från Office 365. Nästa fas i processen kommer att borttagningen av Access Web-databaser som använder SharePoint-listor som deras underliggande datalagring.

**Hur påverkar det här mig?**

Från juni 2019 kan vi avbryta skapandet av nya Access-databaser i SharePoint Online och avsluta tjänsten och eventuella återstående apps April 2020.

**Vad behöver jag göra för att förbereda för den här ändringen?**

Vi rekommenderar att du skapar en plan för övergång för organisationens Access web-databaser. Administratörer kan använda [skanner för åtkomst till SharePoint-app](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) för att hämta en inventering av Access apps webbplatser använder.

Det finns flera sätt att migrera data för Access web-databaser:

- Importera lokala Access-databaser (. ACCDB) eller till en Excelfil.
- Vi rekommenderar också att utforska Microsoft PowerApps som en alternativ plattform för att skapa affärslösningar med ingen kod för webben och mobila enheter.