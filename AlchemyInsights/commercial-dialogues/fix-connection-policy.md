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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988230"
---
# <a name="fix-connection-policy"></a>Åtgärda anslutningsprincip

E-postmeddelandet har markerats som säkert och levererats till användarens inkorg eftersom den avsändande IP-adressen markerades som säker i principen för anslutningsfilter. Så här granskar du principen:

1. Gå till [Office 365 säkerhets- & säkerhets-](https://go.microsoft.com/fwlink/p/?linkid=2077143)och efterlevnadscenter och gå **sedan** till Policy för hothantering  >    >  [mot skräppost.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. På fliken **Anpassad** väljer du **Anslutningsfilterprincip** och sedan **Redigera princip**.
3. Granska listan **över tillåtna IP-adresser.** Se om **Valv är** aktiverad.

    > [!NOTE]
    > Microsoft prenumererar på tredjepartskällor för betrodda avsändare. Om **Valv här** listan är aktiverad markeras inte dessa betrodda avsändare av misstag som skräppost. Jag rekommenderar att du väljer det här alternativet eftersom det minskar antalet falska positiva resultat (bra e-postmeddelanden som klassificeras som skräppost) som du får.
