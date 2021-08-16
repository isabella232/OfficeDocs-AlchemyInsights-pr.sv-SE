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
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030812"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP kan behöva en anpassad typ

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP kan kräva en anpassad informationstyp**

Med en DLP-princip (Data Loss Prevention) kan du identifiera och skydda känsliga data i organisationen. I vissa fall kan du behöva skapa en egen **anpassad** typ av känslig information för att skydda organisationens data.

Din organisation kan till exempel behöva identifiera och skydda anställnings-ID eller andra data i ett format som är specifikt för din organisation. I så fall finns mer information i följande artiklar.
  
 **Anpassa en inbyggd typ av känslig information**
  
Om en inbyggd typ av känslig information skulle uppfylla dina behov med några få justeringar kan du anpassa en inbyggd typ av [känslig information.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Du kan till exempel lägga till eller ta bort nyckelord eller lägga till eller ta bort stödbevis, till exempel ett datum eller en adress.
  
 **Skapa en anpassad känslig informationstyp**
  
Men om du behöver identifiera och skydda en annan typ av känslig information helt och hållet kan du skapa en anpassad typ av [känslig information](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) i användargränssnittet i Säkerhets- och & Efterlevnadscenter.
  
**Skapa en anpassad typ av känslig information i Säkerhets- och efterlevnadscenter PowerShell**

Om användargränssnittet inte innehåller alla alternativ som du behöver kan du skapa en anpassad typ av känslig information i [Security & Compliance Center PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) Genom att börja med en XML-fil kan du använda alla tillgängliga alternativ.
