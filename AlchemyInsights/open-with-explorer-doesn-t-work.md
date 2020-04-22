---
title: Öppna med Explorer fungerar inte
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713052"
---
# <a name="open-with-explorer-isnt-working"></a>Öppna med Explorer fungerar inte

Om **Öppna med Utforskaren** eller **Visa i Utforskaren** inte fungerar kontrollerar du att WebClient-tjänsten är inställd **på Kör** genom att följa stegen nedan. Det kan till exempel ta lång tid att öppna ett SharePoint- eller OneDrive-bibliotek när tjänsten inte körs. 
  
1. Skriv kör i sökrutan i Windows, välj appen Kör skrivbord, skriv services.msc och välj sedan **Retur**.
    
2. Bläddra ned till WebClient-tjänsten och kontrollera kolumnen **Status.** Om WebClient-tjänstens status inte **körs**dubbelklickar du på Tjänsten, klickar på **Start**och sedan på **OK**. Aktivera tjänsten om det behövs genom att välja **manuell** eller **automatisk** i rutan **Starttyp.** 
    
> [!NOTE]
> Mer om du vill felsöka problem som öppnas i Utforskaren finns [i Öppna i Utforskaren](https://go.microsoft.com/fwlink/?linkid=871665). Utforska synkronisering som ett bättre alternativ: [Synkronisera SharePoint-filer med den nya OneDrive-synkroniseringsklienten](https://go.microsoft.com/fwlink/?linkid=871666). 
  

