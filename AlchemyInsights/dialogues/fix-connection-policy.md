---
title: Åtgärda anslutningsprincipen
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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695889"
---
# <a name="fix-connection-policy"></a>Åtgärda anslutningsprincipen

E-postmeddelandet har markerats som säkert och levererats till användarens inkorg eftersom den avsändande IP-adressen har markerats som säker i principen för anslutningsfilter. Så här granskar du principen:

1. Gå till [Säkerhets- och efterlevnadscenter & Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)och gå **sedan** till Policy för skydd mot  >    >  [skräppost.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Välj **anslutningsfilterprincipen** på **fliken Anpassad** och välj sedan **Redigera princip.**
3. Granska listan **över tillåtna IP-adresser.** Se om **listan Över säkra är** aktiverad.

    > [!NOTE]
    > Microsoft prenumererar på källor från tredje part med betrodda avsändare. Om **listan Över** betrodda avsändare har aktiverats markeras inte dessa som skräppost av misstag. Jag rekommenderar att du väljer det här alternativet eftersom det minskar antalet falska positiva meddelanden (bra e-postmeddelanden som klassificeras som skräppost) som du får.
