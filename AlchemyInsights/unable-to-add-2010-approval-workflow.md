---
title: Det gick inte att lägga till 2010 Godkännandearbetsflöde
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049571"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Det gick inte att lägga till 2010 Godkännandearbetsflöde

I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbetsflöde (till exempel "godkännande-SharePoint 2010") i en lista eller ett bibliotek.
  
Lös problemet så här: 
  
1. Öppna rotwebbplatsen för webbplatssamlingen i SharePoint Designer 2013.
  
2. Under **platsobjekt**väljer du **arbetsflöden**. 
  
3. I det **nya** avsnittet i menyfliksområdet för **arbetsflöden** väljer du **återanvändbart arbetsflöde**. 
  
4. I formuläret **skapa återanvändbart arbetsflöde** anger du namnet * * *Repair2010* * *. För **plattformstyp**klickar du på **SharePoint 2010 Workflow**och sedan på **OK**. 
  
1. Välj **publicera**i avsnittet **Spara** i menyfliksområdet för **arbetsflöde** . 
  
2. Välj **publicera globalt**i avsnittet **Hantera** i menyfliksområdet för **arbetsflöde** . I bekräftelsedialogrutan som visas väljer du **OK**. 
  
3. Leta reda på webbplatssamlingens rotwebbplats i en webbläsare och öppna sedan webbplats **samlingens funktioner**för webbplats **Inställningar** \> . Växla funktionen **arbetsflöden** : 
  
· Om funktionen är *aktiverad* klickar du på **inaktivera** och sedan på **Aktivera**. 
  
· Om funktionen är *inaktive* rad klickar du på **Aktivera**. 
  
För mer information hänvisas till följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

