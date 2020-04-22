---
title: Det gick inte att aktivera arbetsflödet som saknades
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762119"
---
# <a name="missing-workflow-failed-to-activate"></a>Det gick inte att aktivera arbetsflödet som saknades

I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbetsflöde (till exempel "Godkännande – SharePoint 2010") i en lista eller ett bibliotek.
  
Så här löser du problemet: 
  
1. Öppna webbplatssamlingens rotwebbplats i SharePoint Designer 2013.
  
2. Under **Webbplatsobjekt**väljer du **Arbetsflöden**. 
  
3. I avsnittet **Nytt** i **menyfliksområdet Arbetsflöden** väljer du **Återanvändbart arbetsflöde**. 
  
4. Ange namnet ** *Repair2010* **i formuläret **Skapa återanvändbart arbetsflöde.** För **plattformstyp**klickar du på **SharePoint 2010-arbetsflöde**och sedan på **OK**. 
  
1. Välj **Publicera** i avsnittet Spara **Publish**i **menyfliksområdet Arbetsflöde** . 
  
2. Välj **Publicera globalt**i avsnittet **Hantera** i menyfliksområdet **Arbetsflöde** . Välj **OK**i bekräftelsedialogrutan som visas . 
  
3. Leta reda på webbplatssamlingens rotwebbplats i en webbläsare och sedan öppna \> **webbplatsinställningar.** **Site Collection Features** Växla sedan **arbetsflödesfunktionen:** 
  
· Om funktionen är *Aktiverad* klickar du på **Inaktivera** och sedan på **Aktivera**. 
  
· Om funktionen är *Inaktiverad* klickar du på **Aktivera**. 
  
Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

