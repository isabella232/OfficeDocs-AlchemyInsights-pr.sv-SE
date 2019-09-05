---
title: Arbetsflödet som saknas kunde inte aktiveras
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753814"
---
# <a name="missing-workflow-failed-to-activate"></a>Arbetsflödet som saknas kunde inte aktiveras

I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbetsflöde (till exempel "godkännande-SharePoint 2010") i en lista eller ett bibliotek.
  
Lös problemet så här: 
  
1. Öppna rotwebbplatsen för webbplatssamlingen i SharePoint Designer 2013.
  
2. Under **platsobjekt**väljer du **arbetsflöden**. 
  
3. I det **nya** avsnittet i menyfliksområdet för **arbetsflöden** väljer du **återanvändbart arbetsflöde**. 
  
4. I formuläret **skapa återanvändbart arbetsflöde** anger du namnet * * *Repair2010* * *. För **plattformstyp**klickar du på **SharePoint 2010 Workflow**och sedan på **OK**. 
  
1. Välj **publicera**i avsnittet **Spara** i menyfliksområdet för **arbetsflöde** . 
  
2. Välj **publicera globalt**i avsnittet **Hantera** i menyfliksområdet för **arbetsflöde** . I bekräftelsedialogrutan som visas väljer du **OK**. 
  
3. Leta reda på webbplatssamlingens rotwebbplats i en webbläsare och öppna sedan webbplats **samlingens funktioner**för webbplats **Inställningar** \> . Växla sedan funktionen **arbetsflöden** : 
  
· Om funktionen är *aktiverad* klickar du på **inaktivera** och sedan på **Aktivera**. 
  
· Om funktionen är *inaktive* rad klickar du på **Aktivera**. 
  
För mer information hänvisas till följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

