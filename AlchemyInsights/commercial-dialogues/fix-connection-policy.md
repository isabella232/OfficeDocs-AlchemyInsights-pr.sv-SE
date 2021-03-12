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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750599"
---
# <a name="fix-connection-policy"></a>Åtgärda anslutningsprincip

E-postmeddelandet har markerats som säkert och levererats till användarens inkorg eftersom den avsändande IP-adressen markerades som säker i principen för anslutningsfilter. Så här granskar du principen:

1. Gå till [Säkerhets- och & Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)och gå sedan **till** Policy för hothantering mot  >    >  [skräppost.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. På fliken **Anpassad** väljer du **Anslutningsfilterprincip** och sedan **Redigera princip**.
3. Granska listan **över tillåtna IP-adresser.** Se efter **om Listan Över säkra** är aktiverad.

    > [!NOTE]
    > Microsoft prenumererar på tredjepartskällor för betrodda avsändare. Om **listan Över** betrodda avsändare är aktiverad markeras inte dessa betrodda avsändare av misstag som skräppost. Jag rekommenderar att du väljer det här alternativet eftersom det minskar antalet falska positiva resultat (bra e-postmeddelanden som klassificeras som skräppost) som du får.
