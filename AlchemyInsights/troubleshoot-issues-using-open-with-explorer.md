---
title: Felsöka problem med öppna med Utforskaren
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
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659076"
---
# <a name="fix-problems-with-open-with-explorer"></a>Åtgärda problem med öppna med Utforskaren

Åtgärda vanliga problem med att öppna ett dokument bibliotek i SharePoint eller OneDrive med kommandot **Öppna med Utforskaren** : 
  
- Använd Internet Explorer 10 eller Internet Explorer 11. **Öppna med Utforskaren** är inte kompatibelt med Microsoft Edge, Google Chrome, Firefox och andra. **Öppna med Utforskaren** är inaktiverat i alla webbläsare utom Internet Explorer. 
    
- **Öppna med Utforskaren** är inte tillgängligt i den moderna versionen för SharePoint-bibliotek. Använd **Visa i Utforskaren** i stället. Välj vyn **visnings alternativ** \> **i Utforskaren**. Visa i Utforskaren är inte kompatibelt med Microsoft Edge, Google Chrome, Firefox och andra. **Visa i Utforskaren** i endast tillgänglig i Internet Explorer. 
    
- Kontrol lera att WebClient-tjänsten körs. Skriv kör i sökrutan i Windows, välj Kör Skriv bords programmet, Skriv Services. msc och tryck sedan på RETUR. Bläddra ned till WebClient-tjänsten och kontrol lera att kolumnen **status** visar "kör". Om det inte gör det dubbelklickar du på tjänsten, klickar på **Start**och sedan på **OK**. (Du kanske måste aktivera tjänsten först genom att välja antingen **manuell** eller **Automatisk** i rutan **Start metod** .) 
    
> [!NOTE]
> Det är praktiskt att öppna ett bibliotek i Utforskaren om du behöver kopiera eller flytta flera filer och mappar en gång, men om du ofta vill arbeta i biblioteket rekommenderar vi att du synkroniserar det. Information om hur du felsöker problem med öppning i Utforskaren finns i [Öppna i Utforskaren](https://go.microsoft.com/fwlink/?linkid=871665). Information om hur du konfigurerar synkronisering finns i [Synkronisera SharePoint-filer med den nya synkroniseringsklienten för OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Mer information finns i artikeln om [hur du använder kommandot "öppna med Utforskaren" för att felsöka problem i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) . 
  

