---
title: Porta Google Chrome-tillägg Microsoft Edge (Chromium)
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
- "8297"
- "9004617"
ms.openlocfilehash: 34ec7e71a2f27eb5b46395876a4d1c903189be1050e523796c9f2a817c20aaa0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973715"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Porta Google Chrome-tillägg Microsoft Edge (Chromium)

Det är enkelt att [porta Google Chrome-tillägg för Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). I de flesta fall behövs bara minimala ändringar för att köra dessa tillägg på Microsoft Edge.

Tilläggs-API:er och manifestnycklar som stöds av Google Chrome är kodkompatibla med Microsoft Edge. Men Microsoft Edge stöder inte tilläggs-API:er chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken och chrome.instanceID.