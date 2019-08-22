---
title: Öppna i Explorer fungerar inte
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538506"
---
# <a name="open-with-explorer-isnt-working"></a>Öppna i Explorer fungerar inte

Om **Öppna med Utforskaren** eller **Visa i File Explorer** inte fungerar kontrollerar du att WebClient-tjänsten är inställd på **Kör** genom att följa stegen nedan. Till exempel kan det ta lång tid att öppna ett bibliotek i SharePoint eller OneDrive när tjänsten inte körs. 
  
1. I rutan Sök i Windows typ kör, Välj Kör stationär app, typ services.msc och välj sedan **RETUR**.
    
2. Rulla ned till WebClient-tjänsten och kontrollera kolumnen **Status** . Om **status för WebClient-tjänsten inte körs,** Dubbelklicka på tjänsten, klicka på **Start**och klicka sedan på **OK**. Aktivera tjänsten, vid behov genom att välja **Manuell** eller **automatisk** i rutan **Startmetod** . 
    
> [!NOTE]
> Felsökning av problem med öppna i File Explorer finns i [Öppna i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Utforska synkronisering som ett bättre alternativ: [synkronisera SharePoint-filer med den nya OneDrive sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666). 
  

