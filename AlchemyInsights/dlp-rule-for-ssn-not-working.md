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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679387"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problem med person nummer

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problem med efter SSN efter**

Har du problem med **data förlust skydd (DLP)** fungerar inte för innehåll som innehåller ett **person nummer (SSN)** när du använder en känslig informations typ i Microsoft 365? Om så är fallet kontrollerar du att innehållet innehåller den information som behövs för att använda DLP-policyn. 
  
För exempelvis en SSN-princip som har kon figurer ATS med en konfidensnivå på 85% utvärderas följande och måste identifieras för att regeln ska utlösa:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 siffror, som kan vara i ett formaterat eller oformaterat mönster

- **[Mönster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Fyra funktioner letar efter efter SSN efter i fyra olika mönster:

  - Func_ssn hittar efter SSN efter med för2011 stark formatering som formaterats med tank streck eller blank steg (DDD-DD-dddd eller DDD mm dddd)

  - Func_unformatted_ssn hittar efter SSN efter med förformaterad formatering som är oformaterad 2011 med nio efterföljande siffror (sssssssss)

  - Func_randomized_formatted_ssn hittar inlägg-2011-efter SSN efter som formaterats med tank streck eller blank steg (DDD-DD-dddd eller DDD mm dddd)

  - Func_randomized_unformatted_ssn hittar efter-2011-efter SSN efter som är oformaterade med nio efterföljande siffror (sssssssss)

- **[Kontroll Summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nej, det finns ingen kontroll Summa

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** En DLP-princip är 85% trygg att den här typen av känslig information identifieras om, inom ett avstånd på 300 tecken:

  - [Funktionen Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) hittar innehåll som matchar mönstret.

  - Ett nyckelord från [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) hittas. Exempel på nyckelord:  *social trygghet, social trygghet #, SOC SEK, SSN*  . Följande exempel skulle till exempel utlösas för policyn DLP SSN: **SSN: 489-36-8350**
  
Mer information om vad som krävs för att efter SSN efter ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [vad den känsliga informations typen letar efter efter SSN efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Om du använder en annan inbyggd känslig informations typ kan du läsa följande artikel för information om vad som är obligatoriskt för andra typer: [vad den känsliga informations typen letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  