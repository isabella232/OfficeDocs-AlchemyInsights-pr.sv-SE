---
title: samma som filnamnet är bäst
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
ms.openlocfilehash: b77e514da36701808d46248e8f2a45137751a1c7
ms.sourcegitcommit: 5447031f9d0a320c49897b8adb5d29ac9437fbc5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/18/2019
ms.locfileid: "35786431"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Obligatoriska Alkemi huvud H1, H2's fungerar inte.
Metodtips och riktlinjer för redigering av Alkemi:

1. **Kapsla inte Alkemi insikter i mappar**- detta bryts url-struktur. Vi söker i åtgärda detta.
1. Filer i mappen **AlchemyInsights** ska ha gemener filnamn med bindestreck för utrymmen ex. ***how-till-aktivera-tvist-Håll***.
    1. Inkludera regel-ID eller bucket-ID från [Alkemi Partner-portalen](https://alchemyportal.azurewebsites.net) i fältet ms.custom. fritt. ***MS.Custom: 100021***
1. Använd resten av metadata överst i den här filen som en mall.
1. I [Alkemi-Partner-portalen](https://alchemyportal.azurewebsites.net), gå till avsnittet **kunden Insight titel:** och användning som pekar som en startpunkt för H1-rubriken för insight. 
    > [!NOTE]
    > Alkemi insikter måste ha bara en enda H1 överst eller de bryts i produktionen. H2s återge inte så Använd **fetstil** eller andra konventioner att tillkännage separata avsnitt.
1. Sedan fyller du i brödtext med utkast material i avsnittet Kund insikter i regel Alkemi-sida
    1. Punktlistor är bra
    1. För numrerade listor
    1. **Fet** och *kursiv stil* är a-ok
    1. Länkar ska alltid vara antingen **”länkar till web” / extern** eller **djup-länkar till gränssnittselement**, inte interna länkar.
    1. Bilder stöds inte officiellt just nu, men det är på plan.

Detta är egentligen redan lite för långt. Bästa praxis är cirka 400 tecken torrsubstanshalt

När innehållet är klar kan du dra den levande grenen. Sedan går du till [Alkemi på partnerportalen](https://alchemyportal.azurewebsites.net) och ange filnamnet i url-fältet. 


