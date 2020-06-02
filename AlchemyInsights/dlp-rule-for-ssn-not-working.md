---
title: DLP-regeln för SSN fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507388"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problem med personnummer

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problem med SSN-nätverk**

Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett **personnummer (SSN)** när du använder en känslig informationstyp i Microsoft 365? Om så är fallet, se till att ditt innehåll innehåller den information som behövs för vad DLP-principen söker. 
  
För en SSN-princip som konfigurerats med en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 siffror, som kan vara i ett formaterat eller oformaterat mönster

- **[Mönster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fyra funktioner letar efter SSN i fyra olika mönster:

  - Func_ssn hittar SSN med stark formatering före 2011 som är formaterad med streck eller blanksteg (ddd-ddd-dddd ELLER ddd dd dddd)

  - Func_unformatted_ssn hittar SSN med stark formatering före 2011 som är oformaterade som nio på varandra följande siffror (ddddddddddddd)

  - Func_randomized_formatted_ssn hittar SSN efter 2011 som är formaterade med streck eller blanksteg (ddd-dddd ELLER ddd ddd ddddd)

  - Func_randomized_unformatted_ssn hittar SSN efter 2011 som är oformaterade som nio på varandra följande siffror (dddddddddddd)

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nej, det finns ingen Kontrollsumma

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-princip är 85 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:

  - [Funktionen Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) hittar innehåll som matchar mönstret.

  - Ett nyckelord från [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) hittas. Exempel på nyckelord är: *Social Security, Social Security #, Soc Sec , SSN* . Följande exempel skulle till exempel utlösa för DLP SSN-principen: **SSN: 489-36-8350**
  
Mer information om vad som krävs för att SSN ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter SSN-nätverk](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  