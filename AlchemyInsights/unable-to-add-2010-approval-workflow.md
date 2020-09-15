---
title: Det går inte att lägga till arbets flödet för 2010-godkännande
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699753"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Det går inte att lägga till arbets flödet för 2010-godkännande

I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbets flöde (som "godkännande-SharePoint 2010") i en lista eller ett bibliotek.
  
Lös problemet genom att följa de här stegen: 
  
1. Öppna webbplatsens rot webbplats i SharePoint Designer 2013.
  
2. Välj **arbets flöden**under **webbplats objekt**. 
  
3. I det **nya** avsnittet i menyfliksområdet **arbets flöden** väljer du **återanvändbart arbets flöde**. 
  
4. Ange namnet * * *Repair2010* * * i formuläret **skapa åter användnings Bart arbets flöde** . För **plattforms typer**klickar du på **SharePoint 2010-arbetsflöde**och sedan på **OK**. 
  
1. Välj **publicera**i avsnittet **Spara** i **arbets flödets** menyfliksområde. 
  
2. I avsnittet **Hantera** i menyfliksområdet **arbets flöde** väljer du **publicera globalt**. Välj **OK**i bekräftelse dialog rutan som visas. 
  
3. I en webbläsare letar du reda på rot webbplatsen för webbplats samlingen och sedan åtkomst till webbplats **Site Settings** \> **samlings funktioner**för webbplats inställningar. Aktivera funktionen **arbets flöden** : 
  
· Om funktionen är  *aktive rad*  klickar **du på Inaktivera och sedan** på **Aktivera**. 
  
· Om funktionen är  *inaktive rad*  klickar du på **Aktivera**. 
  
Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

