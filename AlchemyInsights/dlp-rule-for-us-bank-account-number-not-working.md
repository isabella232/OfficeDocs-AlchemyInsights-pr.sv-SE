---
title: DLP-regel för AMERIKANSKt bankkonto nummer fungerar inte
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679314"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problem med amerikanska bank konto nummer

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problem med amerikanska bank konto nummer**

Har du problem med **data förlust skydd (DLP)** fungerar inte för innehåll som innehåller ett **amerikanskt bankkonto nummer** när du använder en typ av DLP-känslig information i O365? I så fall bör du kontrol lera att innehållet innehåller den information som behövs för att DLP-policyn ska identifieras när den utvärderas.
  
Om till exempel en policy för **amerikansk bank konto nummer** har kon figurer ATS med en konfidensnivå på 85% utvärderas följande och måste identifieras för att regeln ska utlösa:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 siffror

- **[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 siffror i följd.

- **[Kontroll Summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, det finns ingen kontroll Summa

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-princip är 75% trygg att den här typen av känslig information identifieras om, inom ett avstånd på 300 tecken:

  - Det reguljära uttrycket Regex_usa_bank_account_number hittar innehåll som matchar mönstret

  - Ett nyckelord från Keyword_usa_Bank_Account hittas.

    Följande exempel skulle till exempel utlösa policyn för **bank konto nummer för USA** för att kontrol lera konto 78344011

Mer information om vad som krävs för att ett **amerikanskt bank konto nummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [vad de känsliga informations typerna ser ut för ditt bank konto nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Om du använder en annan inbyggd känslig informations typ kan du läsa följande artikel för information om vad som är obligatoriskt för andra typer: [vad den känsliga informations typen letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  