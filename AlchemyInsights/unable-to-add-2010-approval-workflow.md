---
title: Det går inte att lägga till arbetsflödet för 2010-godkännande
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: e74c842f8b4be321664f8c2f1f58c570d0724d80edb1264add0647bf313bc82f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020354"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Det går inte att lägga till arbetsflödet för 2010-godkännande

I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbetsflöde (till exempel "Godkännande - SharePoint 2010") i en lista eller ett bibliotek.
  
Lös problemet genom att följa de här stegen: 
  
1. Öppna rotwebbplatsen för webbplatssamlingen i SharePoint Designer 2013.
  
2. Välj **Arbetsflöden** under **Webbplatsobjekt.** 
  
3. I avsnittet **Nytt** i menyfliksområdet **Arbetsflöden** väljer du **Återanvändbart arbetsflöde.** 
  
4. I formuläret **Skapa återanvändbart arbetsflöde** anger du namnet ** *Reparera2010* **. För **Plattformstyp** klickar du **SharePoint 2010-arbetsflöde** och sedan på **OK.** 
  
1. I avsnittet **Spara** i menyfliksområdet **Arbetsflöde** väljer du **Publicera.** 
  
2. I avsnittet **Hantera** i menyfliksområdet **Arbetsflöde** väljer du **Publicera globalt.** Välj OK i bekräftelsedialogrutan som **visas.** 
  
3. Leta reda på rotwebbplatsen i webbplatssamlingen i en webbläsare och öppna sedan **Webbplatssamling Inställningar** \> **Webbplatssamlingens funktioner.** Växla funktionen **Arbetsflöden:** 
  
· Om funktionen är *aktiverad klickar* du på **Inaktivera och** sedan på **Aktivera.** 
  
· Om funktionen är *inaktiverad klickar* du på **Aktivera.** 
  
Mer information finns i följande [artikel.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

