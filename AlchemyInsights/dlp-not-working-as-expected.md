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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707828"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerar inte som förväntat

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Konfigurera DLP**

Fungerar du inte som **förväntat med DLP (Data Loss Prevention)** i Office 365? I så fall kontrollerar du att **DLP-principen** är korrekt konfigurerad och att dina data innehåller det **som DLP-principen** letar efter när den utvärderas.
  
Med DLP-principer kan du identifiera och skydda känslig information i organisationen. Om du vill konfigurera DLP-principer använder du informationen [här.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Vad DLP-principer söker efter**
  
När du använder de inbyggda typerna för känslig information i Center för säkerhet och efterlevnad söker **DLP-principerna** efter specifika mönster och element när dessa känsliga typer identifieras.
  
- **Inbyggda typer av känslig information**

    Mer information om inbyggda typer av känslig information och vad en DLP-princip söker efter när typen Känslig identifieras finns i: Vilka typer av [känslig information letar du efter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Anpassade typer av känslig information**

    Om du vill skapa anpassade typer av känslig information kan du använda följande artikel för information om hur du skapar en anpassad typ av känslig information: Skapa en anpassad [typ av känslig information.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testa en DLP-princip**

Om du vill testa dina data med en inbyggd  eller anpassad typ av känslig information använder du alternativet Testtyp under **Klassificeringar**–  >  **känslig information.** Mer information finns i Testa [anpassade typer av känslig information.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Rapporter**
  
- Få känsliga datainsikter [med DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Visa specifik information om händelsen med en [incidentrapport.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
