---
title: samma som filnamn är bäst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/15/2019
ms.locfileid: "35800063"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Krävs Alchemy header H1, H2's fungerar inte.
Bästa praxis och riktlinjer för Alchemy författande:

1. **Inte kapsla Alchemy insikter i mappar**-detta kommer att bryta URL-strukturen. Vi tittar på att fixa detta.
1. Filer i mappen **Alchemyinsights** ska ha gemener filnamn med bindestreck för blanksteg ex. ***hur-till-möjliggöra-rättstvist-Hold***.
    1. Inkludera regel-ID eller Bucket-ID från [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net) i den MS. Custom fält. Ex. ***MS Custom: 100021***
1. Använd resten av metadata överst i den här filen som din mall.
1. I [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net), Navigera ner till avsnittet **kundinsikt titel:** och använda det som en utgångspunkt för din H1 titel för insikten. 
    > [!NOTE]
    > Alchemy Insights måste ha bara en enda H1 på toppen eller de kommer att bryta i produktionen. H2S gör inte heller så Använd **fetstil** eller andra konventioner för att beteckna separata sektioner.
1. Fyll sedan i brödtexten med hjälp av utkasts materialet i avsnittet Customer Insights på sidan Alchemy Rule
    1. Punktlistor är bra
    1. Numrerade listor för
    1. **Fet** och *kursiv* är a-OK
    1. Länkar ska alltid vara antingen **"länkar till webb"/externa** eller **djupa länkar till UI element**, inte interna länkar.
    1. Bilder stöds inte officiellt vid denna tid, men det är på färdplanen.

Och detta är verkligen redan lite för länge. Bästa praxis är cirka 400 tecken---------------------------------

När innehållet är klart drar du det till grenen Live. Gå sedan till [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net) och ange filnamnet i URL-fältet. 