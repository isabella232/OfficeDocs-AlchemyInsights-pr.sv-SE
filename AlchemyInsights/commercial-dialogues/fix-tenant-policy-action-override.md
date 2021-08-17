---
title: Åtgärda klientprincip (åsidosättning av åtgärder)
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
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896093"
---
# <a name="fix-tenant-policy-action-override"></a>Åtgärda klientprincip (åsidosättning av åtgärder)

En av dina principer mot skräppost påverkade det här meddelandet. Så här granskar du principerna:

1. Gå Microsoft 365 Defender principer för samarbete &-post och & principer för hot mot skräppost i avsnittet Principer i webbportalen för <https://security.microsoft.com/>  \>  \>  \> **e-Microsoft 365 Defender.** 

   Om du vill gå direkt till sidan **Principer för skräppostskydd** använder du <https://security.microsoft.com/antispam>.

2. På sidan Principer för skydd mot skräppost markerar du principen genom att klicka på namnet på principen **(Typ** är Custom **anti-spam** policy eller **Name** is **Anti-Spam inbound policy (Default)**). 
3. I den utfällade informationen som visas väljer **du Redigera** åtgärder i **avsnittet** Åtgärder.
4. I avsnittet **Meddelandeåtgärder** granskar du omdömena **för skräppost,** skräppost  med hög konfidens, nätfiske och nätfiske med hög konfidens för att se om något av följande värden är markerat:  
   - **Lägg till X-sidhuvud**
   - **Förbereda ämnesraden med text**
   - **Omdirigera meddelandet till e-postadress**
   - **Ta bort meddelande**
   - **Ingen åtgärd**

   Det är möjligt att **standardinställningarna som tillämpats** på alla Exchange Online Protection påverkade meddelandet.

Mer information finns i [Konfigurera principer för skräppostskydd i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
