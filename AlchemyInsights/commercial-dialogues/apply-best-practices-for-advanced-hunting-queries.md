---
title: Använda metodtips för avancerade sökfrågor
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749550"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Använda metodtips för avancerade sökfrågor

Använd de här metodtipsen för att få resultat snabbare och undvika tidsgränser när du kör komplexa frågor:

- När du försöker med nya frågor ska du alltid använda en gräns, för att undvika att få extremt stora resultatuppsättningar. Använd också `count` för att göra en första bedömning av storleken på resultatuppsättningen.
- Använd tidsfilter först. Under idealiska tider bör du begränsa dina frågor till sju dagar.
- I början av en fråga, direkt efter tidsfiltret, lägger du till de filter som förväntas ta bort de flesta data.
- När du söker efter fullständiga token ska du använda `has` operatorn i stället för `contains` .
- Kör en sökning på en specifik kolumn i stället för i alla kolumner.
- När du sammanfogar tabeller ska du först ange tabellen med färre rader.
- `project` endast de kolumner som behövs i tabellerna som du har anslutit till.

Mer information finns i Avancerad [frågedesign.](https://go.microsoft.com/fwlink/?linkid=2144812)
