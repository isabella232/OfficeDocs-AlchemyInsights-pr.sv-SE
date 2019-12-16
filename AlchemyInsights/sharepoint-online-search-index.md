---
title: Sök i SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044061"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Innehåll genomsökning och indexering i SharePoint Online

Innehållet måste crawlas och läggas till i sökindexet för att användarna ska kunna hitta det de söker efter i SharePoint Online. Innehållet crawlas automatiskt baserat på ett fördefinierat crawlningsschema (crawlningsschemat kan inte ändras). Crawlern plockar upp innehåll som har ändrats sedan den senaste crawlningen och uppdaterar indexet. Observera följande för att säkerställa att innehållet crawlas och indexet uppdateras:

- Se till att innehållet kan hittas genom [att göra webbplatsens innehåll sökbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- När du har ändrat en hanterad egenskap, eller när du har ändrat mappningen av crawlade och hanterade egenskaper, måste platsen crawlas igen innan ändringarna återspeglas i sökindexet. 

    Eftersom dina ändringar görs i sökschemat, och inte på den faktiska platsen, indexerar inte crawlern automatiskt webbplatsen. 

    Mer information finns [i begära genomsökning och Omindexering av en webbplats, ett bibliotek eller en lista manuellt](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Vänta minst 24 timmar efter att du manuellt begärt en crawlning och ett fullständigt nytt index för att se om problemet kvarstår. 

    Om mer än 24 timmar har gått sedan du initierade crawlningen och fullständig re-index, vänligen logga ett supportärende. I många fall arbetar vi redan på en lösning. Vänligen ge oss minst 24 timmar för att slutföra en lösning.

> [!IMPORTANT]
> Om en webbplats, ett dokument (bibliotek) eller en lista har tagits bort och fortfarande visas i sökresultaten, bör användare få ett **fel 404 filen hittades inte** när du försöker komma åt den. Det här problemet bör loggas som ett supportärende för ytterligare utredning. 



