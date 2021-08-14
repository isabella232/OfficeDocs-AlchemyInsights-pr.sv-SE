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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930151"
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
