---
title: Öppna med Utforskaren fungerar inte
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694474"
---
# <a name="open-with-explorer-isnt-working"></a>Öppna med Utforskaren fungerar inte

Om **Öppna med Utforskaren** eller **vyn i Utforskaren** inte fungerar kontrollerar du att WebClient-tjänsten är inställd på att **köras** genom att följa stegen nedan. Det kan ta lång tid att öppna ett SharePoint-eller OneDrive-bibliotek när tjänsten inte körs. 
  
1. Skriv kör i sökrutan i Windows, välj Kör Skriv bords programmet, Skriv Services. msc och välj sedan **RETUR**.
    
2. Bläddra ned till WebClient-tjänsten och kontrol lera kolumnen **status** . Om WebClient-tjänstens status inte **körs**dubbelklickar du på tjänsten, klickar på **Start**och sedan på **OK**. Aktivera tjänsten, om det behövs genom att välja **manuellt** eller **automatiskt** i rutan **Start** . 
    
> [!NOTE]
> Information om hur du felsöker problem med öppning i Utforskaren finns i [Öppna i Utforskaren](https://go.microsoft.com/fwlink/?linkid=871665). Utforska synkroniseringen som ett bättre alternativ: [Synkronisera SharePoint-filer med den nya synkroniseringsklienten för OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

