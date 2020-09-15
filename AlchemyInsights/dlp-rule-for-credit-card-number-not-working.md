---
title: DLP-regel för kreditkorts nummer fungerar inte
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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679459"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problem med kreditkorts nummer

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problem med kreditkorts nummer**

Har du problem med **data förlust skydd (DLP)** fungerar inte för innehåll som innehåller ett **kreditkorts nummer** när du använder en DLP-känslig informations typ i O365? Om så är fallet kontrollerar du att innehållet innehåller den information som behövs för att utlösa DLP-principen när den utvärderas. För att en **kredit korts princip** är konfigurerad med en konfidensnivå på 85% utvärderas till exempel följande och måste identifieras för att regeln ska utlösa:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 siffror som kan formateras eller formateras (ssssssssssssssss) och måste godkänna Luhn-testet.

- **[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Mycket komplext och robust mönster som identifierar kort från alla större varumärken, inklusive Visa, MasterCard, Discover-kort, JCB, American Express, presentkort och betalkort-kort.

- **[Kontroll Summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Ja, Luhn, kontroll Summa

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** En DLP-princip är 85% trygg att den här typen av känslig information identifieras om, inom ett avstånd på 300 tecken:

  - Funktionen Func_credit_card hittar innehåll som matchar mönstret.

  - Något av följande stämmer:

  - Ett nyckelord från Keyword_cc_verification hittas.

  - Ett nyckelord från Keyword_cc_name hittas

  - Funktionen Func_expiration_date hittar ett datum i rätt datum format.

  - Kontroll summan passerar

    Följande exempel skulle till exempel utlösa en policy för DLP-kreditkorts nummer:

  - Visa: 4485 3647 3952 7352
  
  - Upphör: 2/2009

Mer information om vad som krävs för att ett **kreditkorts nummer** ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [vad den känsliga informations typen letar efter kreditkort #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Om du använder en annan inbyggd känslig informations typ kan du läsa följande artikel för information om vad som är obligatoriskt för andra typer: [vad den känsliga informations typen letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  