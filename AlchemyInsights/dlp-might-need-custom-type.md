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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446709"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP kan behöva en anpassad typ

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP kan kräva en anpassad informationstyp**

Med en DLP-princip (Data Loss Prevention) kan du identifiera och skydda känsliga data i organisationen. I vissa fall kan du behöva skapa en egen anpassad typ av känslig information för att skydda organisationens data. Mer information finns i Läs [mer om typer av känslig information](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) och definitioner av typer av känslig [information.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Mer information om hur du skapar anpassade typer och principer för känslig information finns i: 

**Anpassa en inbyggd typ av känslig information**

Om en inbyggd typ av känslig information skulle uppfylla dina behov med bara några justeringar kan du gå till Anpassa en inbyggd typ av [känslig information.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Du kan till exempel lägga till eller ta bort nyckelord eller lägga till eller ta bort stödbevis, till exempel ett datum eller en adress.

**Skapa en anpassad känslig informationstyp**

Men om du behöver identifiera och skydda en annan typ av känslig information helt och hållet kan du skapa en anpassad typ av känslig information i Microsoft 365 Efterlevnadscenter. Mer information finns i Komma [igång med anpassade typer av känslig information.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Skapa en anpassad typ av känslig information i Säkerhets- och efterlevnadscenter PowerShell**

Slutligen kan du skapa en anpassad typ av känslig information i Security & Compliance Center PowerShell om användargränssnittet inte innehåller alla alternativ som du behöver. Genom att börja med en XML-fil kan du använda alla tillgängliga alternativ. Mer information finns i Skapa [en anpassad typ av känslig information med PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Om du vill testa principen i testläge först kan du gå till Implementera princip i [testläge](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) och [Skapa, testa och finjustera en DLP-princip.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 