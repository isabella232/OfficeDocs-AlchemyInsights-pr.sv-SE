---
title: Det går inte att lägga till arbetsflöde för godkännande av 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 3741b1169ddf731725c18fbaed80bfb321e5db46
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32366853"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Det går inte att lägga till arbetsflöde för godkännande av 2010

Du kan inte lägga till ett globalt återanvändbart arbetsflöde (till exempel ”godkännande - SharePoint 2010”) i en Microsoft SharePoint-webbplatssamling till en lista eller ett bibliotek.
  
Lös problemet så här: 
  
1. Öppna webbplatsen för webbplatssamlingen rot i SharePoint Designer 2013.
  
2. Välj **arbetsflöden**under **Platsobjekt**. 
  
3. Välj **Återanvändbart arbetsflöde**i avsnittet **Nytt** i menyfliksområdet för **arbetsflöden** . 
  
4. Ange namnet på formuläret **Skapa återanvändbart arbetsflöde** ** *Repair2010* **. Klicka på **SharePoint 2010 arbetsflöde**för **Plattformstyp**och klicka på **OK**. 
  
1. Välj **Publicera**i avsnittet **Spara** i menyfliksområdet för **arbetsflöde** . 
  
2. Välj **Publicera globalt**i avsnittet **Hantera** i menyfliksområdet för **arbetsflöde** . Välj **OK**i dialogrutan för bekräftelse. 
  
3. Hitta webbplatssamlingen rot webbplats i en webbläsare och tillgång till **Webbplatsinställningar** \> **Webbplatssamlingens funktioner**. Växla funktionen **arbetsflöden** : 
  
· Om funktionen är *aktiverad* , klickar du på **inaktivera,** och klicka sedan på **Aktivera**. 
  
· Om funktionen är *Inaktiverad* kan du klicka på **Aktivera**. 
  
Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

