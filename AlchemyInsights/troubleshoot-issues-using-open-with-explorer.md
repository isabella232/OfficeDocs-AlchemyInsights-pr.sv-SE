---
title: Felsöka problem med öppna med Utforskaren
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742751"
---
# <a name="fix-problems-with-open-with-explorer"></a>Åtgärda problem med öppna med Utforskaren

Åtgärda vanliga problem med att öppna ett dokumentbibliotek i SharePoint eller OneDrive med kommandot **Öppna med Utforskaren** : 
  
- Använd Internet Explorer 10 eller 11 i Internet Explorer. **Öppna med Utforskaren** är inte kompatibel med Microsoft Edge, Google Chrome, Firefox och andra. **Öppna med Utforskaren** är inaktiverat i alla webbläsare utom Internet Explorer. 
    
- **Öppna med Utforskaren** är inte tillgänglig i den moderna upplevelsen för SharePoint-bibliotek. Använd **Visa i Utforskaren** i stället. Välj **Visa alternativ** \> **i Utforskaren**. Visa i Utforskaren är inte kompatibel med Microsoft Edge, Google Chrome, Firefox och andra. **Visa i Utforskaren** i endast tillgänglig i Internet Explorer. 
    
- Kontrollera att WebClient-tjänsten körs. I Windows-sökrutan skriver du kör, väljer Kör skrivbordsapp, skriver Services. msc och trycker på RETUR. Rulla ned till WebClient-tjänsten och kontrollera att kolumnen **status** visar "löpning". Om den inte gör det dubbelklickar du på tjänsten, klickar på **Start**och sedan på **OK**. (Du måste kanske först aktivera tjänsten genom att välja antingen **manuell** eller **Automatisk** i rutan **Startmetod** .) 
    
> [!NOTE]
> Att öppna ett bibliotek i Utforskaren är praktiskt om du behöver kopiera eller flytta flera filer och mappar en gång, men om du vill arbeta regelbundet i biblioteket rekommenderar vi att du synkroniserar den. Om du vill felsöka problem med att öppna i Utforskaren, se [Öppna i Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Information om hur du konfigurerar synkronisering finns [i Synka SharePoint-filer med den nya OneDrive-synkroniseringsklienten](https://go.microsoft.com/fwlink/?linkid=871666).
  
Se artikeln [hur du använder kommandot "öppna med Utforskaren" för att felsöka problem i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) för mer information. 
  

