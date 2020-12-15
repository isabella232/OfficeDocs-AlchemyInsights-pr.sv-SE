---
title: Port Google Chrome-tillägg till Microsoft Edge (krom)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678980"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Port Google Chrome-tillägg till Microsoft Edge (krom)

Det är lätt att [Porta Google Chrome-tilläggen till Microsoft Edge (krom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). I de flesta fall behövs bara minimala ändringar för att köra dessa tillägg på Microsoft Edge.

De tilläggs-API: er och manifest nycklar som stöds av Google Chrome är kod-kompatibla med Microsoft Edge. Microsoft Edge stöder emellertid inte tilläggens API: er Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken och Chrome. instanceID.