---
title: Saknas arbetsflödet kunde inte aktiveras
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543943"
---
# <a name="missing-workflow-failed-to-activate"></a>Saknas arbetsflödet kunde inte aktiveras

Du kan inte lägga till ett globalt återanvändbart arbetsflöde (till exempel ”godkännande - SharePoint 2010”) i en Microsoft SharePoint-webbplatssamling till en lista eller ett bibliotek.
  
Lös problemet så här: 
  
1. Öppna webbplatsen för webbplatssamlingen rot i SharePoint Designer 2013.
  
2. Välj **arbetsflöden**under **Platsobjekt**. 
  
3. Välj **Återanvändbart arbetsflöde**i avsnittet **Nytt** i menyfliksområdet för **arbetsflöden** . 
  
4. Ange namnet på formuläret **Skapa återanvändbart arbetsflöde** ** *Repair2010* **. Klicka på **SharePoint 2010 arbetsflöde**för **Plattformstyp**och klicka på **OK**. 
  
1. Välj **Publicera**i avsnittet **Spara** i menyfliksområdet för **arbetsflöde** . 
  
2. Välj **Publicera globalt**i avsnittet **Hantera** i menyfliksområdet för **arbetsflöde** . Välj **OK**i dialogrutan för bekräftelse. 
  
3. Hitta webbplatssamlingen rot webbplats i en webbläsare och tillgång till **Webbplatsinställningar** \> **Webbplatssamlingens funktioner**. Växla sedan funktionen **arbetsflöden** : 
  
· Om funktionen är *aktiverad* , klickar du på **inaktivera,** och klicka sedan på **Aktivera**. 
  
· Om funktionen är *Inaktiverad* kan du klicka på **Aktivera**. 
  
Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

