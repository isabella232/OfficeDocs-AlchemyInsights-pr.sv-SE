---
title: Aktivera NDI-teknik
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935194"
---
# <a name="turn-on-ndi-technology"></a>Aktivera NDI-teknik

NDI-teknik kräver två steg för att aktiveras för en användare:

1. Administratören för klientorganisationen måste aktivera egenskapen AllowNDIStreaming i CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. När ändringen har fyllts i måste slutanvändaren aktivera NDI® för sin specifika klient från **Inställningar > Behörigheter.**

Mer information finns i Använda [NDI-teknik i Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
