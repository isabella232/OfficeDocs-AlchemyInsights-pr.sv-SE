---
title: DLP fungerar inte som förväntat
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679711"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerar inte som förväntat

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Konfigurera DLP**

Har du problem med **data förlust (DLP)** i Office 365 inte fungerar som det ska? Om så är fallet, se till att **DLP-principen** är korrekt konfigurerad och att dina data innehåller den information som används för att använda DLP- **principen** när den utvärderas.
  
Med DLP-principer kan du identifiera och skydda känslig information i organisationen. Använd informationen [här](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)för att konfigurera DLP-principer.
  
 **Vilka DLP-principer som ska sökas efter**
  
När du använder de **inbyggda känsliga informations typerna** i säkerhets-och EFTERLEVNADSPRINCIPER kan DLP-principer leta efter specifika mönster och element när de här känsliga typerna identifieras.
  
- **Inbyggda känsliga informations typer**

    Information om de inbyggda känsliga typerna och vilken DLP-princip som används för att identifiera den känsliga typen finns i: [vad den känsliga informations typen letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Anpassade typer av känslig information**

    Om du försöker skapa anpassade informations typer kan du använda följande artikel för att få information om hur du skapar en anpassad känslig typ: [skapa en anpassad känslig informations typ](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testa en DLP-princip**

Om du vill testa dina data med en inbyggd eller anpassad känslig informations typ använder du alternativet **testtyp** under **klassificerings**  >  **känsliga informations typer**. Mer information finns i [testa anpassade typer av känslig information](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapporter**
  
- Få känsliga data insikter med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Visa detaljerad information om händelsen med en [incident rapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
