---
title: Felsöka problem med Öppna med Utforskaren
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759710"
---
# <a name="fix-problems-with-open-with-explorer"></a>Åtgärda problem med Öppna med Utforskaren

Åtgärda vanliga problem med att öppna ett dokumentbibliotek i SharePoint eller OneDrive med kommandot **Öppna med Utforskaren:** 
  
- Använda Internet Explorer 10 eller Internet Explorer 11. **Öppna med Explorer** är inte kompatibelt med Microsoft Edge, Google Chrome, Firefox och andra. **Öppna med Explorer** är inaktiverat i alla webbläsare utom Internet Explorer. 
    
- Det går inte att **öppna med Utforskaren** i den moderna upplevelsen för SharePoint-bibliotek. Använd **Visa i Utforskaren i** stället. Välj **Visa alternativ** \> **Visa i Utforskaren**. Visa i Utforskaren är inte kompatibel med Microsoft Edge, Google Chrome, Firefox och andra. **Visa i Utforskaren** endast tillgängligt i Internet Explorer. 
    
- Kontrollera att WebClient-tjänsten körs. Skriv kör i sökrutan i Windows, välj appen Kör skrivbord, skriv services.msc och tryck sedan på Retur. Bläddra ned till WebClient-tjänsten och se till att **kolumnen Status** visar "Körs". Om den inte gör det dubbelklickar du på tjänsten, klickar på **Start**och sedan på **OK**. (Du kan behöva aktivera tjänsten först genom att välja **Manuell** eller **Automatisk** i rutan **Starttyp.)** 
    
> [!NOTE]
> Det är praktiskt att öppna ett bibliotek i Utforskaren om du behöver kopiera eller flytta flera filer och mappar en gång, men om du vill arbeta regelbundet i biblioteket rekommenderar vi att du synkroniserar det. Mer om du vill felsöka problem som öppnas i Utforskaren finns [i Öppna i Utforskaren](https://go.microsoft.com/fwlink/?linkid=871665). Information om hur du konfigurerar synkronisering finns i [Synkronisera SharePoint-filer med den nya OneDrive-synkroniseringsklienten](https://go.microsoft.com/fwlink/?linkid=871666).
  
Mer information finns i artikeln [Så här använder du kommandot "Öppna med Utforskaren" för att felsöka problem i SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 
  

