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
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011354"
---
# <a name="open-with-explorer-isnt-working"></a>Öppna med Utforskaren fungerar inte

Om Öppna med  **Utforskaren** eller Visa i Utforskaren inte fungerar kontrollerar du att WebClient-tjänsten är inställd på **Körs** genom att följa stegen nedan. Det kan till exempel ta lång tid att öppna SharePoint eller OneDrive biblioteket när tjänsten inte körs. 
  
1. I sökrutan Windows du kör, väljer programmet Kör skrivbord, skriver services.msc och väljer sedan **Ange**.
    
2. Bläddra ned till WebClient-tjänsten och kontrollera **kolumnen** Status. Om WebClient-tjänstens status **inte körs** dubbelklickar du på tjänsten, klickar på **Starta** och klickar sedan på **OK.** Aktivera tjänsten om det behövs genom att välja **antingen Manuell** **eller** Automatisk **i rutan Starttyp.** 
    
> [!NOTE]
> Information om hur du felsöker problem med att öppna i [Utforskaren finns i Öppna i Utforskaren.](https://go.microsoft.com/fwlink/?linkid=871665) Utforska synkronisering som ett bättre alternativ: [synkronisera SharePoint filer med den nya OneDrive-synkronisering klienten](https://go.microsoft.com/fwlink/?linkid=871666). 
  

