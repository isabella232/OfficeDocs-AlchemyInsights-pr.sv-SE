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
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530315"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerar inte som förväntat

Har du problem med **Data förlust Prevention (DLP)** i Office 365 fungerar inte som förväntat? Om så är fallet, kontrollera att din **DLP princip** har konfigurerats korrekt och att dina data innehåller vilken **DLP princip** söker efter när det utvärderas.
  
 **Ställa in DLP**
  
DLP-principer kan du identifiera och skydda känslig information i din organisation. Inställningar för DLP-principer genom att använda informationen [här](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **DLP-principer leta efter**
  
När du använder **inbyggda känslig informationstyper** i Office 365 säkerhet och överensstämmelse center leta DLP principer efter särskilda mönster och element när upptäcka sådana känsliga.
  
- **Typer av inbyggda känslig Information**

    Information om de inbyggda känsliga typerna och en DLP-princip ser för när identifiera känsliga typen finns: [letar du vilka av känslig information](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Typer av anpassade känslig Information**

    Om du vill skapa anpassade känslig information, Använd följande artikel för information om hur du skapar en anpassad känsliga typ: [Skapa en anpassad känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Testa en DLP-princip**

Om du vill testa dina data med en inbyggd eller anpassad känslig information använder du alternativet **Testa typ** under **klassificeringar** > **informationstyper av känslig**. Mer information finns i [anpassade känslig information testtyper](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapporter**
  
- Hämta känsliga data insikter med [DLP rapporter.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Se specifika detaljer om händelsen med en [Rapport om incidenten](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
