---
title: DLP-regel för kreditkortsnummer fungerar inte
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
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389595"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problem med kreditkortsnummer

Har du problem med **Data förlust Prevention (DLP)** fungerar inte för innehåll som innehåller ett **Kreditkortsnummer** när du använder en DLP känslig informationstyp i O365? Om så är fallet, kontrollera innehållet innehåller informationen som krävs för att utlösa den DLP-principen när det utvärderas. Till exempel ett **kreditkort princip** konfigureras med en konfidensnivå på 85%, följande utvärderas och måste identifieras att utlösa regeln:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 siffror som kan vara formaterad eller oformaterad (dddddddddddddddd) och måste klara Luhn-testet.

- **[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Mycket komplexa och robust mönster som identifierar kort från alla stora varumärken över hela världen, inklusive Visa, MasterCard, Discover-kort, JCB, American Express, presentkort och diner-kort.

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, Luhn-kontrollsumma

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** En DLP-princip är 85% säker på att den har upptäckt att den här typen av känslig information om inom ett avstånd av 300 tecken:

  - Funktionen Func_credit_card returnerar innehåll som matchar mönstret.

  - Något av följande är sant:

  - Det finns ett nyckelord från Keyword_cc_verification.

  - Ett nyckelord från Keyword_cc_name hittades

  - Funktionen Func_expiration_date söker efter ett datum i formatet rätt datum.

  - Kontrollsumman passerar

    Till exempel initierar i följande exempel principens DLP kreditkort nummer:

  - Visa: 4485 3647 3952 7352
  
  - Förfaller: 2/2009

Mer information om vad som krävs för ett **Kreditkortsnummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad den känsliga informationstyper leta efter kreditkort #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Med en annan inbyggd känslig information-typ finns i följande artikel för information om vad som krävs för andra typer: [vad den känsliga informationstyper leta efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  