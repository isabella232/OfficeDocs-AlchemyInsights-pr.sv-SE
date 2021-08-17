---
title: Åtgärda anslutningsprincip
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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888424"
---
# <a name="fix-connection-policy"></a>Åtgärda anslutningsprincip

E-postmeddelandet har markerats som säkert och levererats till användarens inkorg eftersom käll-IP-adressen markerades som säker i standardprincipen för anslutningsfilter. Så här granskar du principen:

1. Gå Microsoft 365 Defender principer för samarbete &-post och & principer för hot mot skräppost i avsnittet Principer i webbportalen för <https://security.microsoft.com/>  \>  \>  \> **e-Microsoft 365 Defender.** 

   Om du vill gå direkt till sidan **Principer för skräppostskydd** använder du <https://security.microsoft.com/antispam>.

2. På sidan **Principer för skydd mot skräppost** markerar du principen med namnet **Anslutningsfilterprincip (standard)** genom att klicka på namnet på principen.

3. Klicka på Redigera anslutningsfilterprincip i **avsnittet Anslutningsfiltrering i** informationsfällfältet **som** visas.

4. Granska posterna i avsnittet Tillåt alltid meddelanden från följande IP-adresser eller **adressintervall** och se om **Aktivera listan Över säkra är** markerad.

   > [!NOTE]
   > Microsoft prenumererar på tredjepartskällor till betrodda avsändare. Om listan över betrodda avsändare har aktiverats markeras inte dessa av misstag som skräppost. Vi rekommenderar att du väljer det här alternativet eftersom det minskar antalet falska positiva resultat (bra e-postmeddelanden som klassificeras som skräppost) som du får.

Mer information finns i [konfigurera anslutningsfilter](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
