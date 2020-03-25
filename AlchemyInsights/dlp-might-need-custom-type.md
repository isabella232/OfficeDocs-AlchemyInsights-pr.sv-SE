---
title: DLP kan behöva en anpassad typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932676"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP kan behöva en anpassad typ

**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden. Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar. Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.

Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid. Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider. Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.

**DLP kan kräva en anpassad informationstyp**

Med en DLP-princip (Data Loss Prevention) kan du identifiera och skydda känsliga data i organisationen. I vissa fall kan du behöva skapa en egen **anpassad** känslig informationstyp för att skydda organisationens data.

Din organisation kan till exempel behöva identifiera och skydda medarbetar-ID:er eller andra data i något format som är specifikt för din organisation. Om så är fallet, se följande artiklar för mer information.
  
 **Anpassa en inbyggd känslig informationstyp**
  
Om en inbyggd känslig informationstyp skulle uppfylla dina behov med bara några justeringar, kan du [anpassa en inbyggd känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Du kan till exempel lägga till eller ta bort nyckelord eller lägga till eller ta bort stödbevis, till exempel ett datum eller en adress.
  
 **Skapa en anpassad känslig informationstyp**
  
Men om du behöver identifiera och skydda en annan typ av känslig information helt och hållet kan du [skapa en anpassad känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) i användargränssnittet i Security & Compliance Center.
  
**Skapa en anpassad känslig informationstyp i Security & Compliance Center PowerShell**

Om användargränssnittet inte innehåller alla alternativ du behöver kan du [slutligen skapa en anpassad känslig informationstyp i Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Genom att börja med en XML-fil kan du använda alla tillgängliga alternativ.
