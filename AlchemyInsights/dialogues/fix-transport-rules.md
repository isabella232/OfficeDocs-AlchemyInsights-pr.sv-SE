---
title: Åtgärda transportregler
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695863"
---
# <a name="fix-transport-rules"></a>Åtgärda transportregler

En anpassad e-postflödesregel påverkade meddelandet. Om du vill granska den exakta regeln gör du följande:

1. Observera **GUID** eller **principnamnet** under Ytterligare information i **resultatet.**
2. Starta Exchange Management Shell. Mer information finns i [Öppna Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Kör det här kommandot (med GUID från din inskickning):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Granska beskrivningen för att se de konfigurerade villkoren som påverkade meddelandet.

Mer information finns i [Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
