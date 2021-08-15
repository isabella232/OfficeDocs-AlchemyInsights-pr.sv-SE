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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023540"
---
# <a name="turn-on-ndi-technology"></a>Aktivera NDI-teknik

NDI-teknik kräver två steg för att aktiveras för en användare:

1. Administratören för klientorganisationen måste aktivera egenskapen AllowNDIStreaming i CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. När ändringen har fyllts i måste slutanvändaren aktivera NDI®-teknik för sin specifika klient från och **Inställningar > behörigheter.**

Mer information finns i Använda [NDI-teknik i Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
