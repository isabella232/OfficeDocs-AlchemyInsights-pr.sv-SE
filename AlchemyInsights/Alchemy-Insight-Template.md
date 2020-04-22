---
title: samma som filnamn är bäst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676551"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Krävs Alchemy Header H1, H2's fungerar inte.
Bästa praxis och riktlinjer för Alchemy författande:

1. **Kapsla inte Alchemy Insights i mappar**- detta kommer att bryta url-strukturen. Vi funderar på att fixa det här.
1. Filer i mappen **AlchemyInsights** bör ha gemener filnamn med bindestreck för blanksteg ex. ***hur-till-aktivera-rättstvist-hold***.
    1. Inkludera regel-ID: t eller bucket-ID:t från [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) i fältet ms.custom. Ex. ***ms.custom: 100021***
1. Använd resten av metadata högst upp i den här filen som mall.
1. I [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net)navigerar du ned till avsnittet **Kundinsiktstitel:** och använd det som utgångspunkt för din H1-titel för insikten. 
    > [!NOTE]
    > Alchemy Insights måste bara ha en enda H1 på toppen eller de kommer att bryta i produktionen. H2s renderar inte antingen så använd **fetstil** eller andra konventioner för att beteckna separata avsnitt.
1. Fyll sedan i brödtexten med hjälp av utkastmaterialet i avsnittet Kundinsikter på sidan Alkemiregel
    1. Punktlistor är bra
    1. Numrerade listor också
    1. **Fet** och *kursiv* är a-ok
    1. Länkar bör alltid vara antingen **"länkar till webben"/externa** eller **djuplänkar till gränssnittselement**, inte interna länkar.
    1. Bilder stöds inte officiellt just nu, men de finns på översikten.

Och detta är egentligen redan lite för lång. Bästa praxis är cirka 400 tecken ---------------------------------

När ditt innehåll är klart drar du det till den levande grenen. Gå sedan till [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) och ange filnamnet i url-fältet. 