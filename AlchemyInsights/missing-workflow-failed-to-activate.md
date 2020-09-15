---
title: Det gick inte att aktivera arbets flödet
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667104"
---
# <a name="missing-workflow-failed-to-activate"></a>Det gick inte att aktivera arbets flödet

I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbets flöde (som "godkännande-SharePoint 2010") i en lista eller ett bibliotek.
  
Lös problemet genom att följa de här stegen: 
  
1. Öppna webbplatsens rot webbplats i SharePoint Designer 2013.
  
2. Välj **arbets flöden**under **webbplats objekt**. 
  
3. I det **nya** avsnittet i menyfliksområdet **arbets flöden** väljer du **återanvändbart arbets flöde**. 
  
4. Ange namnet * * *Repair2010* * * i formuläret **skapa åter användnings Bart arbets flöde** . För **plattforms typer**klickar du på **SharePoint 2010-arbetsflöde**och sedan på **OK**. 
  
1. Välj **publicera**i avsnittet **Spara** i **arbets flödets** menyfliksområde. 
  
2. I avsnittet **Hantera** i menyfliksområdet **arbets flöde** väljer du **publicera globalt**. Välj **OK**i bekräftelse dialog rutan som visas. 
  
3. I en webbläsare letar du reda på rot webbplatsen för webbplats samlingen och sedan åtkomst till webbplats **Site Settings** \> **samlings funktioner**för webbplats inställningar. Sedan kan du växla mellan **arbets flödes** funktionen: 
  
· Om funktionen är  *aktive rad*  klickar **du på Inaktivera och sedan** på **Aktivera**. 
  
· Om funktionen är  *inaktive rad*  klickar du på **Aktivera**. 
  
Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

