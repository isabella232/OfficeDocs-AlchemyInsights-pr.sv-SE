---
title: Innehållet visas inte i Sök resultaten för SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713148"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Innehållet visas inte i Sök resultaten för SharePoint

Följ de här fel söknings stegen när förväntat innehåll inte visas i Sök Resultat:
  
1. Kontrol lera att **webbplatsen** som innehåller förväntat innehåll är inställd på att tillåta att innehåll visas i Sök resultaten. Följ stegen i [Visa innehåll på en webbplats i Sök resultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Kontrol lera att **listan** eller **biblioteket** som innehåller förväntat innehåll är inställd på att tillåta att innehåll visas i Sök resultaten. Följ stegen i [Visa innehåll från listor eller bibliotek i Sök resultaten](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Kontrol lera att layouten för sidan, dokumentet eller den anpassade sidan är publicerad som **huvud version.** Följ steg 3 i [sökningen returnerar inte alla resultat i SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Kontrol lera att användaren har **behörighet** att visa innehållet. Följ stegen i [förstå behörighets nivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Om sökschemat har ändrats genom att lägga till en ny hanterad egenskap genom att redigera en hanterad egenskap, eller genom att ta bort en hanterad egenskap, krävs en crawlning och ett nytt index. **Indexera** om innehållet genom att följa stegen i [manuell crawlning och Omindexering av en webbplats, ett bibliotek eller en lista](https://docs.microsoft.com/sharepoint/crawl-site-content). Det kan ta en stund att vänta 24 timmar innan du kontrollerar resultatet igen.

För mer information, se [Aktivera innehåll på en webbplats för att vara sökbar](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
