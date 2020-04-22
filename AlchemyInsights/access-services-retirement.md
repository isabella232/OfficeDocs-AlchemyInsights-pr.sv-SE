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
# <a name="access-services-retirement"></a>Tillgång till tjänster pensionering

Som vi ursprungligen tillkännagav i MC97576, i mars 2017, och fortsatte att kommunicera under det senaste året access services dras tillbaka. Nästa fas i den här processen blir borttagningen av Access-webbdatabaser som använder SharePoint-listor som underliggande datalagring.

**Hur påverkar detta mig?**

Från och med juni 2019 kommer vi att sluta skapa nya Access-databaser i SharePoint Online och stänga av tjänsten och eventuella återstående appar senast i april 2020.

**Vad behöver jag göra för att förbereda mig för den här ändringen?**

Vi rekommenderar att du skapar en övergångsplan för organisationens Access-webbdatabaser. Administratörer kan använda [SharePoint Access-appskannern](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) för att få en inventering av Access-apparna som webbplatserna använder.

Det finns flera sätt att migrera Data i Access-webbdatabaser:

- Importera till en lokal Access-databas (. ACCDB) eller till en Excel-fil.
- Vi rekommenderar också att du utforskar Microsoft PowerApps som en alternativ plattform för att skapa lösningar utan kod för webb- och mobila enheter.