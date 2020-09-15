---
title: DLP kan behöva en anpassad typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712202"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP kan behöva en anpassad typ

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP kan kräva en anpassad informations typ**

Med en policy för att förhindra data förlust (DLP) kan du identifiera och skydda känslig information i organisationen. I vissa fall kan du behöva skapa en **egen känslig informations** typ för att skydda organisationens data.

Din organisation kan till exempel behöva identifiera och skydda anställnings-ID eller andra data i vissa format som är specifika för din organisation. Om så är fallet, se följande artiklar för mer information.
  
 **Anpassa en inbyggd typ av känslig information**
  
Om en inbyggd känslig informations typ uppfyller dina behov med bara några få saker kan du [Anpassa en inbyggd känslig informations typ](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Du kan till exempel lägga till eller ta bort nyckelord eller lägga till eller ta bort stöd bevis, till exempel ett datum eller en adress.
  
 **Skapa en anpassad känslig informations typ**
  
Men om du behöver identifiera och skydda en annan typ av känslig information kan du [skapa en anpassad känslig informations typ](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) i användar gränssnittet för säkerhets & efterlevnad.
  
**Skapa en anpassad känslig informations typ i säkerhets & Compliance Center PowerShell**

Om användar gränssnittet inte tillhandahåller alla alternativ du behöver kan du [skapa en anpassad känslig informations typ i säkerhets & kompabilitets Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Genom att börja med en XML-fil kan du använda alla tillgängliga alternativ.
