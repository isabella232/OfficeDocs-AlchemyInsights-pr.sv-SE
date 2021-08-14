---
title: DLP-regel för SSN fungerar inte
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005000"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problem med personnummer

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problem med SSN**

Har du problem med **dataförlustskydd (DLP)** fungerar inte för innehåll som innehåller **ett SSN (Social Security Number)** när du använder en typ av känslig information i Microsoft 365? I så fall kontrollerar du att innehållet innehåller den information som behövs för det som DLP-principen letar efter. 
  
För en SSN-princip som till exempel har en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 siffror, som kan vara i ett formaterat eller oformaterat mönster

- **[Mönster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fyra funktioner söker efter SSN i fyra olika mönster:

  - Func_ssn söker efter SSN med stark formatering före 2011 som är formaterade med streck eller blanksteg (s-ss-s eller s)

  - Func_unformatted_ssn söker efter SSN med stark formatering före 2011 som är oformaterade som nio siffror i följd (sss)

  - Func_randomized_formatted_ssn söker efter SSN efter 2011 som är formaterade med streck eller blanksteg (s-ss-s eller s s)

  - Func_randomized_unformatted_ssn söker efter SSN efter 2011 som är oformaterade som nio siffror i följd (ss)

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nej, det finns ingen Kontrollsumma

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-princip har med 85 % säkerhet identifierat den här typen av känslig information om följande inifrån 300 tecken:

  - Funktionen [för Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) hittar innehåll som matchar mönstret.

  - Ett nyckelord [från Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) hittas. Exempel på nyckelord är:  *Social Security, Social Security#, Soc Sec , SSN*  . Följande exempel utlöser till exempel DLP SSN-principen: **SSN: 489-36-8350**
  
Mer information om vad som krävs för att SSN ska identifieras för innehållet finns i följande avsnitt i den här artikeln: Vad typer av känslig information letar [efter SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Om du använder en annan inbyggd typ av känslig information hittar du information om vad som krävs för andra typer av känslig information i följande artikel: Vilka typer av [känslig information letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  