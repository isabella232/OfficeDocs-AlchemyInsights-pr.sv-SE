---
title: Innehållet visas inte i SharePoint-sökresultat
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705679"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Innehållet visas inte i SharePoint-sökresultat

Följ de här felsökningsstegen när förväntat innehåll inte visas i sökresultaten:
  
1. Kontrollera att **webbplatsen** som innehåller det förväntade innehållet är inställd på att tillåta att innehåll visas i sökresultaten. Följ stegen i [Visa innehåll på en webbplats i sökresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontrollera att **listan** eller **biblioteket** som innehåller det förväntade innehållet är inställt på att tillåta att innehåll visas i sökresultaten. Följ stegen i [Visa innehåll från listor eller bibliotek i sökresultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontrollera att sidan, dokumentet eller den anpassade sidlayouten har publicerats som en **huvudversion.** Följ steg 3 i [Sök returnerar inte alla resultat i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Kontrollera att användaren har **behörighet** att visa innehållet. Följ stegen i [Förstå behörighetsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Om sökschemat har ändrats genom att lägga till en ny hanterad egenskap, genom att redigera en hanterad egenskap eller genom att ta bort en hanterad egenskap krävs det att begära en crawlning och indexera om. **Indexera** om innehållet genom att följa stegen i [Manuellt begära crawlning och omindexering av en webbplats, ett bibliotek eller en lista](https://docs.microsoft.com/sharepoint/crawl-site-content). Detta kan ta ett tag, vänta 24 timmar innan du kontrollerar resultaten igen.

Mer information finns i [Aktivera innehåll på en webbplats som ska vara sökbart](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
