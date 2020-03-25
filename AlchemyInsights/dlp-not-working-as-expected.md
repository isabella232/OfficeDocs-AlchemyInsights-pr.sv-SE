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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932640"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerar inte som förväntat

**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden. Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar. Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.

Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid. Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider. Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.

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
