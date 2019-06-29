---
title: Innehåll visas inte i sökresultaten i SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363841"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Innehåll visas inte i sökresultaten i SharePoint

Följ dessa felsökningsåtgärder förväntade innehåll inte visas i sökresultat:
  
1. Kontrollera att **platsen** som innehåller det förväntade innehållet anges att innehållet ska visas i sökresultaten. Följ stegen i [Visa innehåll på en webbplats i sökresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontrollera att **listan** eller **biblioteket** som innehåller det förväntade innehållet anges att innehållet ska visas i sökresultaten. Följ stegen i [Visa innehåll från listor eller bibliotek i sökresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontrollera sidan, dokumentet eller anpassad sidlayout har publicerats som en **huvudversion.** Följ steg 3 i [sökningen inte returnera alla resultat i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Kontrollera att användaren har **behörighet** att visa innehållet. Följ stegen i [Så här fungerar behörighetsnivåer i SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
    
5. Om Sök-schemat har ändrats genom att lägga till en ny hanterad egenskap, redigera en hanterad egenskap eller ta bort en hanterad egenskap som begär en crawlning och indexera kommer att krävas. **Indexera** innehåll genom att följa stegen i [begäran manuellt och crawlning omindexering av en webbplats, ett bibliotek eller en lista](https://docs.microsoft.com/sharepoint/crawl-site-content). Detta kan ta en stund, vänta 24 timmar innan du kontrollerar resultatet igen.

Mer information finns i [Aktivera innehåll på en webbplats ska vara sökbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
