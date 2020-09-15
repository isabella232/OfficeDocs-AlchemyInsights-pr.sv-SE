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
# <a name="access-services-retirement"></a>Dragning av Access Services

Som vi presenterade ursprungligen annonserade i MC97576 mars 2017 och fortsatte att kommunicera under det tidigare året Access Services håller på att avvecklas. Nästa steg i processen kommer att ta bort Access-webbdatabaser som använder SharePoint-listor som sin underliggande data lagring.

**Hur påverkar detta mig?**

Från och med den 2019 juni kommer vi att sluta skapa nya Access-databaser i SharePoint Online och stänga av tjänsten och eventuella återstående appar från april 2020.

**Vad behöver jag göra för att förbereda den här ändringen?**

Vi uppmuntrar dig att skapa ett över gångs abonnemang för organisationens Access-webbdatabaser. Administratörer kan använda [program skannern för SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) för att få en inventering av de Access-appar som webbplatser använder.

Det finns flera sätt att migrera webb databas data från Access:

- Importera till en lokal Access-databas (. ACCDB) eller till en Excel-fil.
- Vi rekommenderar också att du utforskar Microsoft PowerApps som en alternativ plattform för att skapa företags lösningar utan kod för webb-och mobila enheter.