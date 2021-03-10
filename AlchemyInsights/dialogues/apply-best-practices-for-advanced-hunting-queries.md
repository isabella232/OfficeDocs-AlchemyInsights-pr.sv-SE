---
title: Tillämpa metodtips för avancerade sökfrågor
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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696082"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Tillämpa metodtips för avancerade sökfrågor

För att få resultat snabbare och undvika timeouts när du kör komplexa frågor kan du använda följande metodtips:

- När du provar nya frågor bör du alltid använda en gräns för att undvika att få extremt stora resultatuppsättningar. Använd även `count` för att göra en första bedömning av storleken på resultatuppsättningen.
- Använd tidsfilter först. Helst bör du begränsa dina frågor till sju dagar.
- I början av en fråga, direkt efter tidsfiltret, lägger du till de filter som förväntas ta bort de flesta data.
- När du letar efter fullständiga tokens använder du `has` operatorn i stället för `contains` .
- Kör en sökning på en specifik kolumn i stället för i alla kolumner.
- När du sammanfogar tabeller måste du först ange tabellen med färre rader.
- `project` Endast nödvändiga kolumner från tabellerna som du har sammanfogat.

Mer information finns i Advanced [hunting query best practices.](https://go.microsoft.com/fwlink/?linkid=2144812)
