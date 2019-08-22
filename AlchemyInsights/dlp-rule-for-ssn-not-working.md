---
title: DLP-regel för SSN fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529890"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problem med personnummer

Har du problem med **Data förlust Prevention (DLP)** fungerar inte för innehåll som innehåller **Social Security Number (SSN))** när du använder en typ av känslig information i Office 365? Om så är fallet, kontrollera innehållet innehåller informationen som krävs för vad DLP-princip söker. 
  
Till exempel för en SSN-princip som konfigurerats med en konfidensnivå på 85% följande utvärderas och måste identifieras att utlösa regeln:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 siffror, som kan vara i en formaterad eller oformaterad mönster

- **[Mönster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fyra funktioner är SSNs i fyra olika mönster:

  - Func_ssn hittas SSNs med pre-2011 starka formatering som är formaterade med streck och blanksteg (ddd-dd-dddd eller ddd dd dddd)

  - Func_unformatted_ssn hittas SSNs med pre-2011 starka formatering som är oformaterad som nio på varandra följande siffror (ddddddddd)

  - Func_randomized_formatted_ssn söker efter inlägg 2011-SSNs som är formaterade med streck och blanksteg (ddd-dd-dddd eller ddd dd dddd)

  - Func_randomized_unformatted_ssn söker efter inlägg 2011-SSNs som är oformaterad som nio på varandra följande siffror (ddddddddd)

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, det finns ingen kontrollsumma

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-princip är 85% säker på att den har upptäckt att den här typen av känslig information om inom ett avstånd av 300 tecken:

  - [Funktionen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) returnerar innehåll som matchar mönstret.

  - Det finns ett nyckelord från [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Innehåller exempel på nyckelord: *Social trygghet, Social trygghet #, Soc sek, SSN* . Till exempel i följande exempel initierar för principen DLP SSN: **SSN: 489-36-8350**
  
Mer information om vad som krävs för SSNs ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad den känsliga informationstyper leta efter SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Med en annan inbyggd känslig information-typ finns i följande artikel för information om vad som krävs för andra typer: [vad den känsliga informationstyper leta efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  