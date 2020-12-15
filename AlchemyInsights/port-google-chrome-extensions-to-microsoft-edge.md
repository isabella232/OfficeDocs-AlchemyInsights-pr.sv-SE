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
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="b036e-102">Port Google Chrome-tillägg till Microsoft Edge (krom)</span><span class="sxs-lookup"><span data-stu-id="b036e-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="b036e-103">Det är lätt att [Porta Google Chrome-tilläggen till Microsoft Edge (krom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="b036e-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="b036e-104">I de flesta fall behövs bara minimala ändringar för att köra dessa tillägg på Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="b036e-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="b036e-105">De tilläggs-API: er och manifest nycklar som stöds av Google Chrome är kod-kompatibla med Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="b036e-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="b036e-106">Microsoft Edge stöder emellertid inte tilläggens API: er Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken och Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="b036e-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>