---
title: Använda distributionsverktyget för Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010889"
---
# <a name="using-the-office-deployment-tool-odt"></a>Använda Office Deployment Tool (ODT)

Du kan använda OFFICE Deployment Tool (ODT) för att distribuera Office 365-versioner av Office. Office Deployment Tool (setup.exe) körs från kommandoraden och använder en XML-fil för konfiguration för att avgöra vilka inställningar som ska gälla vid distribution av Office.
  
1. Hämta den senaste versionen av Distributionsverktyget för Office från [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Använd [Office Customization Tool (OCT)](https://config.office.com) för att välja distributionsinställningar och skapa konfigurations-XML-filen. Exportera konfigurationsfilen och placera den lokalt i samma mapp där setup.exe finns.

    **Anm.:** Problem med Office-installation uppstår ofta på grund av felkonfigurerade eller felformaterade konfigurationsfiler. För att undvika sådana problem rekommenderar vi att du använder Anpassningsverktyget för Office för att skapa konfigurationsfilen. Du kan också importera befintliga konfigurationsfiler till Anpassningsverktyget för Office.

3. Från en upphöjd kommandotolk växlar du till den plats där setup.exe finns och kör Office Deployment Tool i nedladdningsläge och anger konfigurationsfilen som du just sparade. I det här exemplet heter konfigurationsfilen Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Kör Office Deployment Tool i konfigurera läge och ange konfigurationsfilen.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Anm.:** Du måste köra det här steget från klientdatorn där du vill installera Office och du måste ha lokala administratörsbehörigheter på den datorn.

Mer information om hur du använder Distributionsverktyg för Office för microsoft 365-appar för företagsdistributionsscenarier finns [i Översikt över Distributionsverktyget för Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Mer information om hur du använder Anpassningsverktyget för Office finns i [Översikt över Anpassningsverktyget för Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
