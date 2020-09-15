---
title: samma som fil namnet är bäst
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
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664152"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Obligatoriskt Alchemy-huvud H1, H2's fungerar inte."
Metod tips och rikt linjer för Alchemy:

1. **Kapsla inte in Alchemy insikter i mappar**– Detta raderar URL-strukturen. Vi håller på att fixa detta.
1. Filer i **AlchemyInsights** -mappen bör ha gemena fil namn med bindestreck. ***instruktion-handhållning***.
    1. Inkludera regel-ID eller Bucket-ID från [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net) i fältet MS. Custom. hand. ***MS. Custom: 100021***
1. Använd resten av metadata högst upp i den här filen som mall.
1. I [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net)navigerar du ned till avsnittet **kund Insight-rubriken:** och använder den som utgångs punkt för din H1-rubrik för inblicken. 
    > [!NOTE]
    > Alchemy-insikter får bara ha en enda H1 högst upp, eller så kommer de att brytas i produktionen. H2S återger vare sig så Använd **fetstil** eller andra konventioner för att ange separata avsnitt.
1. Fyll i bröd texten med hjälp av utkastet i avsnittet Customer Insights på Alchemy-regel Sidan
    1. Det är bra att Visa punkt listor
    1. Numrerade listor också
    1. **Fetstil** och *kursiv stil* är a-OK
    1. Länkar ska alltid vara antingen **"länkar till webb"/External** eller **djupa länkar till gränssnitts element**, inte interna länkar.
    1. Bilder stöds inte för närvarande, men är på översikten.

Och det är alldeles för långt. Bästa metod är att 400 tecken---------------------------------

När innehållet är klart drar du det till den levande grenen. Gå sedan till [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net) och ange fil namnet i fältet URL. 