---
title: DLP-regel för oss bankkontonummer fungerar inte
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529901"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problem med oss bankkontonummer

Har du problem med **Data förlust Prevention (DLP)** fungerar inte för innehåll som innehåller ett **Bankkontonummer för USA** när du använder en DLP känslig informationstyp i O365? Om så är fallet kontrollerar du att ditt innehåll innehåller informationen som krävs för vilka principen DLP söker efter när det utvärderas.
  
Till exempel för en **Amerikansk bankkontonummer** princip som konfigurerats med en konfidensnivå på 85% följande utvärderas och måste identifieras att utlösa regeln:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 siffror

- **[Mönster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 på varandra följande siffror.

- **[Kontrollsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nej, det finns ingen kontrollsumma

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** En DLP-princip är 75% säker på att den har upptäckt att den här typen av känslig information om inom ett avstånd av 300 tecken:

  - Hittar innehåll som matchar mönstret för det reguljära uttrycket Regex_usa_bank_account_number

  - Det finns ett nyckelord från Keyword_usa_Bank_Account.

    Till exempel i följande exempel initierar principens **Amerikanska bankkontonummer** : checkkonto 78344011

Mer information om vad som krävs för **USA bankkontonumret** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [Vad den känsliga informationstyper leta efter amerikanska bankkontonummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Med en annan inbyggd känslig information-typ finns i följande artikel för information om vad som krävs för andra typer: [vad den känsliga informationstyper leta efter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  