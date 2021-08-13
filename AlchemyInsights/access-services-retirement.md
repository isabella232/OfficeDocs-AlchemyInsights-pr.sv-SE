---
title: Åtkomsttjänster kommer tillbaka
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938713"
---
# <a name="access-services-retirement"></a>Åtkomsttjänster kommer tillbaka

Som vi ursprungligen meddelade i MC97576, i mars 2017, och fortsätter att kommunicera under det senaste året Access Services kommer att dras tillbaka. Nästa steg i den här processen är att ta bort Access-webbdatabaser som använder SharePoint-listor som underliggande datalagring.

**Hur påverkar det här mig?**

Från och med juni 2019 kommer vi att sluta skapa nya Access-databaser i SharePoint Online och avsluta tjänsten och eventuella återstående appar senast i april 2020.

**Vad behöver jag göra för att förbereda mig inför ändringen?**

Vi rekommenderar att du skapar en övergångsplan för organisationens Access-webbdatabaser. Administratörer kan använda [Access SharePoint appskannern för](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) att skaffa en inventering av Access-apparna som webbplatser använder.

Det finns flera sätt att migrera data i Access-webbdatabaser:

- Importera till en lokal Access-databas (. ACCDB) eller till en Excel fil.
- Vi rekommenderar också att du utforskar Microsoft PowerApps som en alternativ plattform för att skapa kodkodade affärslösningar för webb- och mobilenheter.