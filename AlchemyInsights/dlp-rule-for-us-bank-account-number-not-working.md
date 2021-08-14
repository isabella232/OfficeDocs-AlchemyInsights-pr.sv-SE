---
title: DLP-regel för bankkontonummer för USA fungerar inte
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
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005036"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problem med bankkontonummer i USA

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problem med bankkontonummer i USA**

Har du problem med dataförlustskydd **(DLP)** fungerar  inte för innehåll som innehåller ett amerikanskt bankkontonummer när du använder en DLP-typ av känslig information i O365? I så fall kontrollerar du att innehållet innehåller den information som behövs för vad DLP-principen letar efter när den utvärderas.
  
För en princip  för bankkontonummer i USA som har en konfidensnivå på 85 % utvärderas följande och måste identifieras för att regeln ska utlösas:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8–17 siffror

- **[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 siffror i följd.

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, det finns ingen Kontrollsumma

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** En DLP-princip har med 75 % säkerhet identifierat den här typen av känslig information om följande inifrån 300 tecken:

  - Det reguljära uttrycket Regex_usa_bank_account_number hittar innehåll som matchar mönstret

  - Ett nyckelord från Keyword_usa_Bank_Account hittas.

    Följande exempel utlöser till exempel den amerikanska principen **Bank Account Number:** Checking Account 78344011

Mer information om vad som  krävs för att ett amerikanskt bankkontonummer ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: Vilka typer av känslig information letar efter [bankkontonummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) i USA
  
Om du använder en annan inbyggd typ av känslig information hittar du information om vad som krävs för andra typer av känslig information i följande artikel: Vilka typer av [känslig information letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  