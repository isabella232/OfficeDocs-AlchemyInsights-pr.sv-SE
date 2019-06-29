---
title: DLP-regel för USA / Storbritannien passnummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 0567e9521507bcc192b187d0e5a8a0658332ff99
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389559"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problem med DLP - USA / Storbritannien Passport tal

Har du problem med **Data förlust Prevention (DLP)** fungerar inte för innehåll som innehåller en **US / UK passnummer** när du använder en DLP känslig informationstyp i O365? Om så är fallet kontrollerar du att ditt innehåll innehåller informationen som krävs för vilka principen DLP söker efter när det utvärderas.
  
Till exempel för en **US / UK passnummer** princip har konfigurerats med en konfidensnivå på 75%, följande utvärderas och måste identifieras för att regeln ska utlösa
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nio siffror

- **[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nio på varandra följande siffror

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, det finns ingen kontrollsumma

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** En DLP-princip är 75% säker på att den har upptäckt att den här typen av känslig information om inom ett avstånd av 300 tecken:

  - Funktionen Func_usa_uk_passport returnerar innehåll som matchar mönstret.

  - Det finns ett nyckelord från Keyword_passport.

    Till exempel i följande exempel initierar för den **US / UK passnummer** princip: amerikanskt pass nummer 123456789

Mer information om vad som krävs för en USA eller Storbritannien passnummer ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [vad den känsliga informationstyper utseende för USA / Storbritannien passnummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Med en annan inbyggd känslig information-typ finns i följande artikel för information om vad som krävs för andra typer: [vad den känsliga informationstyper leta efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  