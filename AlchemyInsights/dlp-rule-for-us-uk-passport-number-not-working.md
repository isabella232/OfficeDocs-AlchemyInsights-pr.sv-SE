---
title: DLP-regel för AMERIKANSKt/brittiska Passport-nummer fungerar inte
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679242"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problem med DLP-amerikanska/brittiska Passport-nummer

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problem med amerikanska/brittiska Passport-nummer**

Har du problem med **data förlust skydd (DLP)** fungerar inte för innehåll som innehåller ett **USA/UK Passport-nummer** när du använder en DLP-känslig informations typ i O365? I så fall bör du kontrol lera att innehållet innehåller den information som behövs för att DLP-policyn ska identifieras när den utvärderas.
  
För att en policy för principer för ett **svenskt och brittiskt nummer** som har kon figurer ATS med en konfidensnivå på 75% utvärderas till exempel följande och måste identifieras för att regeln ska utlösa
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nio siffror

- **[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nio siffror i följd

- **[Kontroll Summa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, det finns ingen kontroll Summa

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-princip är 75% trygg att den här typen av känslig information identifieras om, inom ett avstånd på 300 tecken:

  - Funktionen Func_usa_uk_passport hittar innehåll som matchar mönstret.

  - Ett nyckelord från Keyword_passport hittas.

    Följande exempel skulle till exempel utlösas för policyn **amerikanska/brittiska pass nummer** : U.S. passport Number 123456789

Mer information om vad som krävs för att ett SVENSKt och brittiska Passport-nummer ska identifieras för ditt innehåll finns i följande avsnitt i den här artikeln: [vad den känsliga informations typen letar efter USA/brittiska pass nummer](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Om du använder en annan inbyggd känslig informations typ kan du läsa följande artikel för information om vad som är obligatoriskt för andra typer: [vad den känsliga informations typen letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  