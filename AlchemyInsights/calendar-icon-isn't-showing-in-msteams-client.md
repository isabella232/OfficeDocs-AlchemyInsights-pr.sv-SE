---
title: Kalender ikonen visas inte i Microsoft Teams-klienten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583928"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Kalender ikonen visas inte i Microsoft Teams-klienten

Fliken **kalender** i Teams kräver åtkomst till en Exchange-postlåda via Exchange Web Services. Exchange-postlådan kan vara online eller lokalt. För onlineanvändare som inte ser fliken **kalender** kontrollerar du att de [är licensierade för en Exchange Online-postlåda och att post lådan är aktive rad](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Om användarna är lokala måste du bekräfta att din hybrid konfiguration är felfri. Använd [Guiden för hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) för felsökning. Observera att [Teams kräver Exchange 2016 CU3 eller senare](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Mer information och fel söknings anvisningar finns i [Felsöka problem med interaktioner i Microsoft Teams och Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
