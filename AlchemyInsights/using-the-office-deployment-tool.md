---
title: Använda distributions verktyget för Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085850"
---
# <a name="using-the-office-deployment-tool-odt"></a>Använda distributions verktyget för Office (ODT)

Du använder Office Deployment Tool (ODT) för att distribuera Office 365-versioner av Office. Distributions verktyget för Office (setupodt.exe) körs från kommando raden och använder en XML-konfigurationsfil för att bestämma vilka inställningar som ska användas vid distribution av Office.
  
1. Ladda ner den senaste versionen av distributions verktyget för Office från [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Använd [verktyget för anpassning av Office (ULT)](https://config.office.com) för att välja distributions inställningar och skapa XML-konfigurationsfilen. Exportera konfigurations filen och placera den lokalt på samma mapp där setupodt.exe finns.

    **Obs!** Problem med Office-installationer uppstår ofta på grund av felkonfigurerade eller malformatted. För att undvika sådana problem rekommenderar vi att du använder verktyget Office-anpassning för att skapa konfigurations filen. Du kan också importera befintliga konfigurationsfiler till verktyget för Office-anpassning.

3. Gå till den plats där setupodt.exe finns i en upphöjd kommando tolk och kör distributions verktyget för Office i nedladdnings läge och ange konfigurations filen du just sparade. I det här exemplet heter konfigurations filen Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. kör distributions verktyget för Office i läget konfiguration och ange konfigurations filen.

```setupodt.exe /configure Configuration.xml```

**Obs!** Du måste köra det här steget från den klient dator där du vill installera Office och måste ha lokal administratörs behörighet på den datorn.

Mer information om hur du använder distributions verktyget för Microsoft 365 för företags distributions scenarier finns i [Översikt över distributions verktyget för Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Mer information om hur du använder verktyget Office-anpassning finns i [Översikt över verktyget Office-anpassning](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
