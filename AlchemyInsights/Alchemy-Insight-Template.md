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
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312843"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Alchemy Header H1, H2-s fungerar inte."
Metodtips och riktlinjer för Alchemy-redigering:

1. **Kapsla inte in Alchemy Insights i mappar**– det här bryter URL-strukturen. Vi försöker lösa det här.
1. Filer i mappen **AlchemyInsights** bör ha gemener filnamn med bindestreck för blanksteg. **_how-to-enable-litigation-hold_**.
    1. Ta med regel-ID eller bucket-ID [från Alchemy-partnerportalen](https://alchemyportal.azurewebsites.net) i det anpassade fältet ms.. t.ex. ***ms.custom: 100021***
1. Använd resten av metadata högst upp i den här filen som mall.
1. I [Alchemy-partnerportalen](https://alchemyportal.azurewebsites.net)navigerar  du ned till avsnittet Kundinsiktstitel: och använder det som utgångspunkt för H1-rubriken för insikten. 

**Obs!** Alchemy Insights BARA ha en enda H1 högst upp, annars bryts produktionen. H2:erna återges inte heller, så använd **fetstil** eller andra konventioner för att beteckna separata avsnitt.
1. Fyll sedan i brödtexten med utkastmaterial i avsnittet Customer Insights på sidan Alchemy-regel
    1. Punktlistor fungerar bra
    1. Numrerade listor också
    1. **Fet** och *kursiv stil* är a-ok
    1. Länkar ska alltid vara **antingen "länkar till webben"/externa** ELLER **djuplänkar till användargränssnittselement**, inte interna länkar.
    1. Bilder har inget officiellt stöd för närvarande, men det finns en översikt.

Och det här är faktiskt lite för långt. Metod bör vara ca 400 tecken ---------------------------------

När innehållet är klart drar du det till live branchen. Gå sedan till [Alchemy-partnerportalen](https://alchemyportal.azurewebsites.net) och ange filnamnet i URL-fältet. 