---
title: DLP fungerar inte som förväntat
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977456"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerar inte som förväntat

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Konfigurera DLP**

Har du problem med **att DLP (Data Loss Prevention)** i Office 365 inte fungerar som förväntat? Om så är fallet, se till att **DLP-principen** är korrekt konfigurerad och att dina data innehåller vad **DLP-principen** söker när den utvärderas.
  
Med DLP-principer kan du identifiera och skydda känslig information i organisationen. Om du vill konfigurera DLP-principer använder du informationen [här](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Vad DLP-principer letar efter**
  
När du använder de **inbyggda känsliga informationstyperna** i Office 365 Security and Compliance Center söker DLP-principer efter specifika mönster och element när du identifierar dessa känsliga typer.
  
- **Inbyggda typer av känslig information**

    Information om de inbyggda känsliga typerna och vad en DLP-princip söker efter när du identifierar typen Känslig finns i: [Vilka känsliga informationstyper som söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Anpassade typer av känslig information**

    Om du försöker skapa anpassade typer av känslig information använder du följande artikel för information om hur du skapar en anpassad känslig typ: [Skapa en anpassad känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Testa en DLP-princip**

Om du vill testa dina data med en inbyggd eller anpassad känslig informationstyp använder du alternativet **Testtyp** under Klassificeringar känsliga **informationstyper** > **Sensitive info types**. Mer information finns i [Testa anpassade typer av känslig information](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapporter**
  
- Hämta känsliga datainsikter med [DLP-rapporter.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Se specifik information om händelsen med en [incidentrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
