---
title: Det går inte att lägga till arbetsflödet för godkännande 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582865"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Det går inte att lägga till arbetsflödet för godkännande 2010

I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbetsflöde (till exempel "Godkännande – SharePoint 2010") i en lista eller ett bibliotek.
  
Så här löser du problemet: 
  
1. Öppna webbplatssamlingens rotwebbplats i SharePoint Designer 2013.
  
2. Under **Webbplatsobjekt**väljer du **Arbetsflöden**. 
  
3. I avsnittet **Nytt** i **menyfliksområdet Arbetsflöden** väljer du **Återanvändbart arbetsflöde**. 
  
4. Ange namnet ** *Repair2010* **i formuläret **Skapa återanvändbart arbetsflöde.** För **plattformstyp**klickar du på **SharePoint 2010-arbetsflöde**och sedan på **OK**. 
  
1. Välj **Publicera** i avsnittet Spara **Publish**i **menyfliksområdet Arbetsflöde** . 
  
2. Välj **Publicera globalt**i avsnittet **Hantera** i menyfliksområdet **Arbetsflöde** . Välj **OK**i bekräftelsedialogrutan som visas . 
  
3. Leta reda på webbplatssamlingens rotwebbplats i en **Site Settings** webbläsare och sedan öppna \> **webbplatsinställningar.** Växla **arbetsflödesfunktionen:** 
  
· Om funktionen är *Aktiverad* klickar du på **Inaktivera** och sedan på **Aktivera**. 
  
· Om funktionen är *Inaktiverad* klickar du på **Aktivera**. 
  
Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

