---
title: Med hjälp av verktyget Office Deployment
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492097"
---
# <a name="using-the-office-deployment-tool-odt"></a>Med hjälp av Office Deployment Tool (ODT)

Du kan använda Office Deployment Tool (ODT) för att distribuera Office 365-versioner av Office. Office Deployment Tool (setup.exe) körs från kommandoraden och använder en XML-konfigurationsfil för att avgöra vilka inställningar som ska gälla när du distribuerar Office.
  
1. Hämta den senaste versionen av Office Deployment Tool på [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. Använd [Verktyget Office-anpassning (ULT)](https://config.office.com) för att välja inställningar för distribution och skapa XML-konfigurationsfilen. Exportera konfigurationsfilen och placera den i samma mapp som setup.exe finns lokalt. 
    
    **Observera:** Office-installationen som ofta uppstår problem förfaller till felkonfigurerad eller konfigurationsfiler för malformatted. För att undvika sådana problem, rekommenderar vi att du använder verktyget Office-anpassning för att skapa konfigurationsfilen. Du kan också importera befintliga konfigurationsfiler till verktyget Office-anpassning. 
    
3. Växla till den plats där setup.exe finns från en kommandotolk och kör verktyget Office Deployment i download-läge och ange den konfigurationsfil som du just har sparat. I det här exemplet heter konfigurationsfilen Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Kör verktyget Office Deployment i Konfigurera läge och ange konfigurationsfilen.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Observera:** Du måste köra det här steget från klientdatorn som du vill installera Office och du måste ha lokal administratörsbehörighet på datorn. 
    
Se [Översikt över Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)om du vill veta mer om hur du använder Office Deployment Tool för dina Office 365 ProPlus distributionsscenarier. Mer information om hur du använder verktyget Office-anpassning finns i [Översikt över verktyget Office-anpassning](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

