---
title: DLP-regeln för us/UK Passport Number fungerar inte
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004964"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problem med DLP - US/UK-passnummer

**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP-problem med amerikanska/brittiska passnummer**

Har du problem med **dataförlustskydd (DLP)** fungerar inte för innehåll som innehåller ett **us/UK-passnummer** när du använder en DLP-typ av känslig information i O365? I så fall kontrollerar du att innehållet innehåller den information som behövs för vad DLP-principen letar efter när den utvärderas.
  
För till exempel en **amerikanska/brittiska** passnummerprincip som konfigurerats med en konfidensnivå på 75 % utvärderas följande och måste identifieras för att regeln ska utlösas
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nio siffror

- **[Mönster:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nio siffror i följd

- **[Kontrollsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nej, det finns ingen Kontrollsumma

- **[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** En DLP-princip har med 75 % säkerhet identifierat den här typen av känslig information om följande inifrån 300 tecken:

  - Funktionen för Func_usa_uk_passport hittar innehåll som matchar mönstret.

  - Ett nyckelord från Keyword_passport hittas.

    Följande exempel utlöste till exempel den **amerikanska/brittiska** passnummerpolicyn: Amerikanska Passport number 123456789

Mer information om vad som krävs för att ett us/UK Passport Number ska identifieras för innehållet finns i följande avsnitt i den här artikeln: Vilka typer av känslig information letar efter [us/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Om du använder en annan inbyggd typ av känslig information hittar du information om vad som krävs för andra typer av känslig information i följande artikel: Vilka typer av [känslig information letar efter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  