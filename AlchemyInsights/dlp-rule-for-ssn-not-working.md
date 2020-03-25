---
title: DLP-regeln för SSN fungerar inte
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
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932554"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problem med personnummer

**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden. Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar. Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.

Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid. Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider. Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.

**DLP-problem med SSN-nätverk**

Har du problem med **att Data Loss Prevention (DLP)** inte arbetar för innehåll som innehåller ett **personnummer (SSN)** när du använder en känslig informationstyp i Office 365? Om så är fallet, se till att ditt innehåll innehåller den information som behövs för vad DLP-principen söker. 
  
För en SSN-princip som konfigurerats med en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 siffror, som kan vara i ett formaterat eller oformaterat mönster

- **[Mönster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fyra funktioner letar efter SSN i fyra olika mönster:

  - Func_ssn hittar SSN med stark formatering före 2011 som är formaterad med streck eller blanksteg (ddd-ddd-dddd ELLER ddd dd dddd)

  - Func_unformatted_ssn hittar SSN med stark formatering före 2011 som är oformaterade som nio på varandra följande siffror (ddddddddddddd)

  - Func_randomized_formatted_ssn hittar SSN efter 2011 som är formaterade med streck eller blanksteg (ddd-dddd ELLER ddd ddd ddddd)

  - Func_randomized_unformatted_ssn hittar SSN efter 2011 som är oformaterade som nio på varandra följande siffror (dddddddddddd)

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nej, det finns ingen Kontrollsumma

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** En DLP-princip är 85 % säker på att den har upptäckt den här typen av känslig information om, i närheten av 300 tecken:

  - [Funktionen Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) hittar innehåll som matchar mönstret.

  - Ett nyckelord från [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) hittas. Exempel på nyckelord är: *Social Security, Social Security #, Soc Sec , SSN* . Följande exempel skulle till exempel utlösa för DLP SSN-principen: **SSN: 489-36-8350**
  
Mer information om vad som krävs för att SSN ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad de känsliga informationstyperna letar efter SSN-nätverk](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Med hjälp av en annan inbyggd känslig informationstyp läser du följande artikel för information om vad som krävs för andra typer: [Vad de känsliga informationstyperna söker efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  