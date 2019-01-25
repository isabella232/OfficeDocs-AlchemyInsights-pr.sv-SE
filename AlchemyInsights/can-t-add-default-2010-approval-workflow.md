---
title: Det går inte att lägga till standard 2010 arbetsflöde för godkännande
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29491867"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Det går inte att lägga till standard 2010 arbetsflöde för godkännande

Du kan inte lägga till ett globalt återanvändbart arbetsflöde (till exempel ”godkännande - SharePoint 2010”) i en Microsoft SharePoint-webbplatssamling till en lista eller ett bibliotek.
  
Lös problemet så här: 
  
1. Öppna webbplatsen för webbplatssamlingen rot i SharePoint Designer 2013.
  
2. Välj **arbetsflöden**under **Platsobjekt**. 
  
3. Välj **Återanvändbart arbetsflöde**i avsnittet **Nytt** i menyfliksområdet för **arbetsflöden** . 
  
4. Ange namnet på formuläret **Skapa återanvändbart arbetsflöde** * **Repair2010***. Välj **Arbetsflöde för SharePoint 2010**för **Plattformstyp**, och välj sedan **OK**. 
  
5. Välj **Publicera**i avsnittet **Spara** i menyfliksområdet för **arbetsflöde** . 
  
6. Välj **Publicera globalt**i avsnittet **Hantera** i menyfliksområdet för **arbetsflöde** . Välj **OK**i dialogrutan för bekräftelse. 
  
7. Hitta webbplatssamlingen rot webbplats i en webbläsare och tillgång till **Webbplatsinställningar** \> **Webbplatssamlingens funktioner**. Växla sedan funktionen **arbetsflöden** : 
  
· Om funktionen är *aktiverad* , klickar du på **inaktivera,** och klicka sedan på **Aktivera**. 
  
· Om funktionen är *Inaktiverad* kan du klicka på **Aktivera**. 
  
Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

