---
title: DLP-regeln för kreditkortsnummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977216"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problem med kreditkortsnummer

**Viktigt:** Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga – Besök [Tillfälliga funktionsjusteringar](https://aka.ms/ODSPAdjustments) för SharePoint Online för mer information.

**DLP-problem med kreditkortsnummer**

Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett **kreditkortsnummer** när du använder en DLP-känslig informationstyp i O365? Om så är fallet, se till att ditt innehåll innehåller den information som behövs för att utlösa DLP-principen när den utvärderas. För en **kreditkortsprincip** som konfigurerats med en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 siffror som kan formateras eller oformateras (ddddddddddddddddd) och måste klara Luhn-testet.

- **[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Mycket komplext och robust mönster som upptäcker kort från alla större märken över hela världen, inklusive Visa, MasterCard, Discover Card, JCB, American Express, presentkort och dinerkort.

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn checksum

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-princip är 85 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:

  - Funktionen Func_credit_card hittar innehåll som matchar mönstret.

  - Ett av följande gäller:

  - Ett nyckelord från Keyword_cc_verification hittas.

  - Ett nyckelord från Keyword_cc_name hittas

  - Funktionen Func_expiration_date hittar ett datum i rätt datumformat.

  - Kontrollsumman passerar

    Följande exempel skulle till exempel utlösa för en DLP-kreditkortsnummerpolicy:

  - Visum: 4485 3647 3952 7352
  
  - Löper ut: 2/2009

Mer information om vad som krävs för att ett **kreditkortsnummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter kreditkort#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  