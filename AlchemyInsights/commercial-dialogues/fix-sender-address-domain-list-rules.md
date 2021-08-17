---
title: Åtgärda Avsändaradress-/domänlistregler
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
ms.openlocfilehash: db8b921fc84f42b6cef1138dca9ad433e648e0a2f10e80927bd5b0222bfeae3b
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896129"
---
# <a name="fix-sender-addressdomain-list-rules"></a>Åtgärda Avsändaradress-/domänlistregler

En av dina principer mot skräppost påverkade det här meddelandet. Meddelandets avsändare finns med i listan Tillåt eller Spärra. Så här granskar du principerna:

1. Gå Microsoft 365 Defender principer för samarbete &-post och & principer för hot mot skräppost i avsnittet Principer i webbportalen för <https://security.microsoft.com/>  \>  \>  \> **e-Microsoft 365 Defender.** 

   Om du vill gå direkt till sidan **Principer för skräppostskydd** använder du <https://security.microsoft.com/antispam>.

2. På sidan Principer för skydd mot skräppost markerar du principen genom att klicka på namnet på principen **(Typ** är Custom **anti-spam** policy eller **Name** is **Anti-Spam inbound policy (Default)**). 
3. I den utfällfältet  med information som visas väljer du Redigera tillåtna och blockerade avsändare och domäner i avsnittet Tillåtna och **blockerade avsändare och** domäner.
4. I avsnittet **Tillåtna** granskar du avsändare och domäner genom att klicka på **Hantera \<nn\> avsändare** eller **Tillåt domäner.**

Mer information finns i [Konfigurera principer för skräppostskydd i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
