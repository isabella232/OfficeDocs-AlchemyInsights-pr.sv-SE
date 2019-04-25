---
title: Felsöka problem med att öppna Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390625"
---
# <a name="fix-problems-with-open-with-explorer"></a>Åtgärda problem med att öppna med Explorer

Åtgärda vanliga problem med att öppna ett dokumentbibliotek i SharePoint eller OneDrive med hjälp av kommandot **Öppna med Utforskaren** : 
  
- Använda Internet Explorer 10 eller 11 för Internet Explorer. **Öppna med Utforskaren** inte är kompatibel med Microsoft Edge, Google Chrome, Firefox och andra. **Öppna med Utforskaren** är inaktiverat i alla webbläsare utom Internet Explorer. 
    
- **Öppna med Utforskaren** är inte tillgänglig i den moderna upplevelsen för SharePoint-bibliotek. Använd **vyn i File Explorer** istället. Välj **Visa alternativ** \> **Visa i File Explorer**. Visa i File Explorer är inte kompatibel med Microsoft Edge, Google Chrome, Firefox och andra. **Visa i File Explorer** i endast i Internet Explorer. 
    
- Kontrollera att WebClient-tjänsten körs. Markera appen som kör Fjärrskrivbord i rutan Windows Sök, kör, Skriv, Skriv services.msc och tryck sedan på RETUR. Rulla ned till WebClient-tjänsten och kontrollera att kolumnen **Status** visar ”kör”. Om den inte dubbelklicka på tjänsten, klicka på **Start**och klicka sedan på **OK**. (Du kanske måste först aktivera tjänsten genom att välja **Manuell** eller **automatisk** i rutan **Startmetod** .) 
    
> [!NOTE]
> Öppna ett bibliotek i File Explorer är praktiskt om du vill kopiera eller flytta flera filer och mappar när, men om du regelbundet arbetar i biblioteket, rekommenderar vi synkroniserar den. Felsökning av problem med öppna i File Explorer finns i [Öppna i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Information om hur du konfigurerar synkronisering finns i [synkronisera SharePoint-filer med den nya OneDrive sync-klienten](https://go.microsoft.com/fwlink/?linkid=871666).
  
Se artikel [hur du använder kommandot ”Öppna med Utforskaren” felsökning av problem i SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) för mer information. 
  

