---
title: Vad kan jag göra om Azure-funktionerna inte fungerar korrekt i Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583781"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Vad kan jag göra om Azure-funktionerna inte fungerar korrekt i Microsoft Edge

Microsoft Edge har [kända problem](https://go.microsoft.com/fwlink/?linkid=2140608) som är relaterade till säkerhets zoner och kan påverka hur Azure-användare loggar in i Windows Admin Center. Om du har problem med att använda Azure-funktioner med Microsoft Edge kan du försöka med följande:

1. Sök efter **Internet-alternativ** på **Start** -menyn och välj det.
2. I dialog rutan **Internet egenskaper** går du till fliken **säkerhet** .
3. Välj zonen **tillförlitliga platser** och välj sedan knappen **stationer** .
4. I dialog rutan **tillförlitliga platser** lägger du till GATEWAYens URL och [https://login.microsoftonline.com](https://login.microsoftonline.com) och och [https://login.live.com](https://login.live.com) väljer sedan **Stäng**.
5. I dialog rutan **Internet egenskaper** går du till fliken **Sekretess** .
6. Välj **Inställningar** i avsnittet **blockering av popup-fönster** . I dialog rutan som öppnas lägger du till gateway-URL: en [https://login.microsoftonline.com](https://login.microsoftonline.com) och och [https://login.live.com](https://login.live.com) väljer sedan **Stäng**.
