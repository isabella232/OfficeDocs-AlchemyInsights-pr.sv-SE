---
title: Tillträdestjänster pensionering
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
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050507"
---
# <a name="access-services-retirement"></a>Tillträdestjänster pensionering

Som vi ursprungligen meddelade i MC97576, i mars 2017, och fortsatte att kommunicera under det gångna året tillgång tjänster håller på att dras tillbaka från Office 365. Nästa fas i den här processen kommer att ta bort Access Web-databaser som använder SharePoint-listor som underliggande datalagring.

**Hur påverkar detta mig?**

Från och med 2019 juni kommer vi att stoppa skapandet av nya Access-databaser i SharePoint Online och stänga av tjänsten och eventuella återstående appar i april 2020.

**Vad behöver jag göra för att förbereda mig för den här ändringen?**

Vi uppmuntrar dig att skapa en övergångsplan för organisationens Access-webbdatabaser. Administratörer kan använda [appskannern för SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) för att få en inventering av de Access-appar som webbplatser använder.

Det finns flera sätt att migrera data för Access Web-databaser:

- Importera till en lokal Access-databas (. ACCDB) eller till en Excel-fil.
- Vi rekommenderar också att du utforskar Microsoft PowerApps som en alternativ plattform för att skapa affärslösningar utan kod för webb-och mobilenheter.