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
ms.openlocfilehash: 25744bee6f3ed06ae67fc3c246c7d64fce9994bb
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320543"
---
# <a name="fix-languageip-filter-policy"></a>Åtgärda policy för språk/IP-filter

En av dina principer mot skräppost påverkade det här meddelandet. Så här granskar du principerna:

1. Gå Microsoft 365 Defender principer för samarbete & e-post och & principer för hot mot skräppost i avsnittet Principer i <https://security.microsoft.com/>  \>  \>  \> webbportalen **för** **e-Microsoft 365 Defender.**

   Om du vill gå direkt till sidan **Principer för skräppostskydd** använder du <https://security.microsoft.com/antispam>.

2. På sidan Principer för skydd mot skräppost markerar du principen genom att klicka på namnet på principen **(Typ** är **Custom anti-spam** policy eller **Name** is **Anti-Spam inbound policy (Default)**). 
3. I den utfällklara  detalj som visas väljer du Redigera tröskelvärde för skräppost och egenskaper i avsnittet Tröskelvärde för **massutskick & egenskaper för skräppost.**
4. I avsnittet **Markera som skräppost** granskar du inställningarna Innehåller specifika **språk** och **Från dessa** länder.

Mer information finns i [Konfigurera principer för skräppostskydd i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
