---
title: Åtgärda policy för språk/IP-filter
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
ms.openlocfilehash: 16aa12120034e1f848e62bab151d8e30b251a29e5727f085300d74ca7b49ca52
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896173"
---
# <a name="fix-languageip-filter-policy"></a>Åtgärda policy för språk/IP-filter

En av dina principer mot skräppost påverkade det här meddelandet. Så här granskar du principerna:

1. Gå Microsoft 365 Defender principer för samarbete &-post och & principer för hot mot skräppost i avsnittet Principer i webbportalen för <https://security.microsoft.com/>  \>  \>  \> **e-Microsoft 365 Defender.** 

   Om du vill gå direkt till sidan **Principer för skräppostskydd** använder du <https://security.microsoft.com/antispam>.

2. På sidan Principer för skydd mot skräppost markerar du principen genom att klicka på namnet på principen **(Typ** är Custom **anti-spam** policy eller **Name** is **Anti-Spam inbound policy (Default)**). 
3. I den utfällklara detalj som visas väljer du Redigera tröskelvärde för **skräppost** och egenskaper i avsnittet Tröskelvärde för **massutskick & skräppost.**
4. I avsnittet **Markera som skräppost** granskar du inställningarna Innehåller specifika **språk** och **Från dessa** länder.

Mer information finns i [Konfigurera principer för skräppostskydd i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
