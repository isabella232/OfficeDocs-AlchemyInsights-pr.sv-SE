---
title: Replikuppsättning
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714585"
---
# <a name="replica-set"></a>Replikuppsättning

AADDS kallas även för den hanterade domänen. Det är faktiskt två domänkontrollanter som körs och underhålls av backend. De två dc-erna innehåller ett huvud-DC och en replikerings-DC. Säkerhetskopior i AADDS (hanterad domän) är en automatiserad process som hanteras av Azure-plattformen. I händelse av ett problem med din hanterade domän kan Azure-supporten hjälpa dig att återställa från säkerhetskopiering.

Du skapar varje uppsättning av repliker i ett virtuellt nätverk. Varje virtuellt nätverk måste peered to every other virtual network that hosts a managed domain's replica set. Den här konfigurationen skapar en nättopologi som stöder katalogreplikering. Ett virtuellt nätverk kan ha stöd för flera replikuppsättningar, förutsatt att varje uppsättning av repliker finns i ett annat virtuellt undernät.

Mer information om replikuppsättningar finns i Concepts [Replica-uppsättningar.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
