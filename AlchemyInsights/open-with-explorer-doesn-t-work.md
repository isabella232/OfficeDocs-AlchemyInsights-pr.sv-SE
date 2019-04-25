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
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419890"
---
# <a name="open-with-explorer-isnt-working"></a>Öppna i Explorer fungerar inte

Om **Öppna med Utforskaren** eller **Visa i File Explorer** inte fungerar kontrollerar du att WebClient-tjänsten är inställd på **Kör** genom att följa stegen nedan. Till exempel kan det ta lång tid att öppna ett bibliotek i SharePoint eller OneDrive när tjänsten inte körs. 
  
1. I rutan Sök i Windows typ kör, Välj Kör stationär app, typ services.msc och välj sedan **RETUR**.
    
2. Rulla ned till WebClient-tjänsten och kontrollera kolumnen **Status** . Om **status för WebClient-tjänsten inte körs,** Dubbelklicka på tjänsten, klicka på **Start**och klicka sedan på **OK**. Aktivera tjänsten, vid behov genom att välja **Manuell** eller **automatisk** i rutan **Startmetod** . 
    
> [!NOTE]
> Felsökning av problem med öppna i File Explorer finns i [Öppna i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Utforska synkronisering som ett bättre alternativ: [synkronisera SharePoint-filer med den nya OneDrive sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666). 
  

