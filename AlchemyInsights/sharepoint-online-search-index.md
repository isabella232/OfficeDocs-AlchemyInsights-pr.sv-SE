---
title: Hantera search ordlistor i SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736070"
---
# <a name="search-in-sharepoint-online"></a>Sök i SharePoint Online

Innehållet måste crawlas och lagts till i sökindexet för användare att hitta vad de söker i SharePoint Online. Innehållet crawlas automatiskt baserat på en fördefinierad crawlningsschema (crawlningsschema inte kan ändras). Crawlern hämtar innehåll som har ändrats sedan den senaste crawlningen och uppdaterar indexet. Följ instruktionerna nedan om du vill kontrollera innehållet crawlas och indexet uppdateras.

Kontrollera att innehållet kan hittas genom att göra innehåll sökbart. Mer information finns i [Aktivera innehåll på en webbplats ska vara sökbart](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).

När du har ändrat en hanterad egenskap, eller när du har ändrat avbildningen av crawlade och hanterade vara egenskaper för webbplatsen crawlade igen innan ändringarna återspeglas i sökindexet. 

Indexera webbplatsen eftersom ändringarna görs i schemat för sökning och inte till den faktiska platsen, kommer crawlern inte automatiskt. 

Mer information finns i [begära manuellt och crawlning omindexering av en webbplats, ett bibliotek eller en lista](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).

 Vänta minst 24 timmar efter att ha begärt manuellt crawla och fullständig indexera och se om du fortfarande har problem. 

Om mer än 24 timmar har gått sedan du påbörjade crawla och fullständig indexera, logga ett supportärende. I många fall kan arbetar vi redan på en lösning. Ge oss minst 24 timmar att slutföra en lösning.

**Viktigt**: om en webbplats, dokument (bibliotek) eller en lista var borttagna och fortfarande visas i sökresultaten, användare får ett fel 404-Filen hittades inte när du försöker komma åt. Det här problemet ska loggas som ett supportärende för vidare utredning. 



