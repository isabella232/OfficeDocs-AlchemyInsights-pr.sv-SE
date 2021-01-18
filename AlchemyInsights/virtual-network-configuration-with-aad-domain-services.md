---
title: Virtuell konfiguration med AAD Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885651"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuell konfiguration med AAD Domain Services

Med den virtuella konfigurationen med AAD Domain Services följer de här anvisningarna: 

1. Kontrol lera din domäns hälsa på Azure-portalen https://aka.ms/aadds-health
2. Kontrollerar NSG för regler som blockerar portar som behövs för att synkronisera i Azure AD Domain Services på portalen https://aka.ms/aadds-networking
3. Se till att ditt virtuella nätverk distribueras i samma Azure-region som din Azure AD Domain Services-hanterade domän.
4. Kontrol lera att du inte har en befintlig domän med samma domän namn tillgängliga i det virtuella nätverket.

Mer information om hur du utformar i Azure Virtual Network för att stödja AAD Domain Services finns i det [virtuella nätverket](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

