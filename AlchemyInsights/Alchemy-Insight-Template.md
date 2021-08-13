---
title: Samma som filnamn är bäst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918919"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Alchemy Header H1, H2-s fungerar inte."
Metodtips och riktlinjer för Alchemy-redigering:

1. **Kapsla inte in Alchemy Insights i mappar**– url-strukturen bryts. Vi försöker lösa det här.
1. Filer i mappen **AlchemyInsights** bör ha gemener filnamn med bindestreck för blanksteg. **_how-to-enable-litigation-hold_**.
    1. Ta med regel-ID eller bucket-ID [från Alchemy-partnerportalen](https://alchemyportal.azurewebsites.net) i det anpassade fältet ms.. t.ex. ***ms.custom: 100021***
1. Använd resten av metadata högst upp i den här filen som mall.
1. I [Alchemy-partnerportalen](https://alchemyportal.azurewebsites.net)navigerar  du ned till avsnittet Kundinsiktstitel: och använder det som utgångspunkt för H1-rubriken för insikten. 
    > [!NOTE]
    > Alchemy Insights ENDAST ha en enda H1 högst upp, annars bryts produktionen. H2:erna återges inte heller, så använd **fetstil** eller andra konventioner för att beteckna separata avsnitt.
1. Fyll sedan i brödtexten med utkastmaterial i avsnittet Customer Insights på sidan Alchemy-regel
    1. Punktlistor fungerar bra
    1. Numrerade listor också
    1. **Fet** och *kursiv stil* är a-ok
    1. Länkar ska alltid vara **antingen "länkar till webben"/externa** ELLER **djuplänkar till användargränssnittselement**, inte interna länkar.
    1. Bilder har inget officiellt stöd för närvarande, men det finns en översikt.

Och det här är faktiskt lite för långt. Metod bör vara ca 400 tecken ---------------------------------

När innehållet är klart drar du det till live branchen. Gå sedan till [Alchemy-partnerportalen](https://alchemyportal.azurewebsites.net) och ange filnamnet i URL-fältet. 