---
title: DLP-regel för kreditkortsnummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005108"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problem med kreditkortsnummer

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problem med kreditkortsnummer**

Fungerar det inte att använda **dataförlustskydd (DLP)** för innehåll som innehåller kreditkortsnummer när du använder en DLP-typ av känslig information i O365?  I så fall kontrollerar du att innehållet innehåller den information som behövs för att utlösa DLP-principen när den utvärderas. För en kreditkortsprincip som till exempel har en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas: 
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 siffror som kan vara formaterade eller oformaterade (sss) och måste vara i Luhn-testet.

- **[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Mycket komplex och robust mönster som identifierar kort från alla större varumärken över hela världen, inklusive Visa, MasterCard, Discover Card, JCB, American Express, presentkort och diner-kort.

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn-kontrollsumma

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-princip har med 85 % säkerhet identifierat den här typen av känslig information om följande inifrån 300 tecken:

  - Funktionen Func_credit_card hittar innehåll som matchar mönstret.

  - Något av följande är sant:

  - Ett nyckelord från Keyword_cc_verification hittas.

  - Ett nyckelord från Keyword_cc_name hittas

  - Funktionen Func_expiration_date hittar ett datum i rätt datumformat.

  - Kontrollsumma passeras

    Följande exempel utlöser till exempel en DLP-princip för kreditkortsnummer:

  - Visa: 4485 3647 3952 7352
  
  - Går ut: 2/2009

Mer information om vad som  krävs för att ett kreditkortsnummer ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: Så här söker typer av känslig [information efter kreditkort#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Om du använder en annan inbyggd typ av känslig information hittar du information om vad som krävs för andra typer av känslig information i följande artikel: Vilka typer av [känslig information letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  