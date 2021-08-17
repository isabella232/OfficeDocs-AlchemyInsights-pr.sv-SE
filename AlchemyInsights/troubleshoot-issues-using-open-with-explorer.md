---
title: Felsöka problem med att använda Öppna med Utforskaren
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048174"
---
# <a name="fix-problems-with-open-with-explorer"></a>Åtgärda problem med Öppna med Utforskaren

Åtgärda vanliga problem med att öppna ett dokumentbibliotek i SharePoint eller OneDrive med **kommandot Öppna med** Utforskaren: 
  
- Använd Internet Explorer 10 eller Internet Explorer 11. **Öppna med Utforskaren** är inte kompatibelt med Microsoft Edge, Google Chrome, Firefox och andra. **Öppna med Utforskaren** är inaktiverat i alla webbläsare utom Internet Explorer. 
    
- **Öppna med Utforskaren** är inte tillgängligt i det moderna använda SharePoint bibliotek. Använd **Visa i Utforskaren i** stället. Välj **Visningsalternativ** \> **Visa i Utforskaren**. Visa i Utforskaren är inte kompatibelt med Microsoft Edge, Google Chrome, Firefox och andra. **Visa i Utforskaren** i endast tillgängligt i Internet Explorer. 
    
- Kontrollera att WebClient-tjänsten körs. I sökrutan Windows du kör, väljer programmet Kör skrivbord, skriver services.msc och trycker sedan på Retur. Bläddra ned till WebClient-tjänsten och kontrollera att **"Körs"** visas i kolumnen Status. Om det inte gör det dubbelklickar du på tjänsten, klickar **på Starta** och sedan på **OK.** (Du kanske först måste aktivera tjänsten genom att välja antingen **Manuell** **eller Automatisk** i **rutan Starttyp.)** 
    
> [!NOTE]
> Att öppna ett bibliotek i Utforskaren är användbart om du behöver kopiera eller flytta flera filer och mappar en gång, men om du vill arbeta regelbundet i biblioteket rekommenderar vi att du synkroniserar det. Information om hur du felsöker problem med att öppna i [Utforskaren finns i Öppna i Utforskaren.](https://go.microsoft.com/fwlink/?linkid=871665) Mer information om hur du inställningar för synkronisering [finns i SharePoint filer med den nya OneDrive-synkronisering klienten.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Mer information finns i [artikeln om hur du använder kommandot "Öppna](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) med Utforskaren" för att felsöka problem i SharePoint Online. 
  

