---
title: DLP-regeln för kreditkortsnummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507424"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problem med kreditkortsnummer

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problem med kreditkortsnummer**

Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett **kreditkortsnummer** när du använder en DLP-känslig informationstyp i O365? Om så är fallet, se till att ditt innehåll innehåller den information som behövs för att utlösa DLP-principen när den utvärderas. För en **kreditkortsprincip** som konfigurerats med en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 siffror som kan formateras eller oformateras (ddddddddddddddddd) och måste klara Luhn-testet.

- **[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Mycket komplext och robust mönster som upptäcker kort från alla större märken över hela världen, inklusive Visa, MasterCard, Discover Card, JCB, American Express, presentkort och dinerkort.

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn checksum

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-princip är 85 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:

  - Funktionen Func_credit_card hittar innehåll som matchar mönstret.

  - Ett av följande gäller:

  - Ett nyckelord från Keyword_cc_verification hittas.

  - Ett nyckelord från Keyword_cc_name hittas

  - Funktionen Func_expiration_date hittar ett datum i rätt datumformat.

  - Kontrollsumman passerar

    Följande exempel skulle till exempel utlösa för en DLP-kreditkortsnummerpolicy:

  - Visum: 4485 3647 3952 7352
  
  - Löper ut: 2/2009

Mer information om vad som krävs för att ett **kreditkortsnummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter kreditkort#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  