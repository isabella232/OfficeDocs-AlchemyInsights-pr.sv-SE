---
title: DLP kan behöva en anpassad typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704507"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP kan behöva en anpassad typ

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP kan kräva en anpassad informationstyp**

Med en DLP-princip (Data Loss Prevention) kan du identifiera och skydda känsliga data i organisationen. I vissa fall kan du behöva skapa en egen **anpassad** känslig informationstyp för att skydda organisationens data.

Din organisation kan till exempel behöva identifiera och skydda medarbetar-ID:er eller andra data i något format som är specifikt för din organisation. Om så är fallet, se följande artiklar för mer information.
  
 **Anpassa en inbyggd känslig informationstyp**
  
Om en inbyggd känslig informationstyp skulle uppfylla dina behov med bara några justeringar, kan du [anpassa en inbyggd känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Du kan till exempel lägga till eller ta bort nyckelord eller lägga till eller ta bort stödbevis, till exempel ett datum eller en adress.
  
 **Skapa en anpassad känslig informationstyp**
  
Men om du behöver identifiera och skydda en annan typ av känslig information helt och hållet kan du [skapa en anpassad känslig informationstyp](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) i användargränssnittet i Security & Compliance Center.
  
**Skapa en anpassad känslig informationstyp i Security & Compliance Center PowerShell**

Om användargränssnittet inte innehåller alla alternativ du behöver kan du [slutligen skapa en anpassad känslig informationstyp i Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Genom att börja med en XML-fil kan du använda alla tillgängliga alternativ.
