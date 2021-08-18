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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326815"
---
# <a name="fix-tenant-policy-action-override"></a>Åtgärda klientprincip (åsidosättning av åtgärder)

En av dina principer mot skräppost påverkade det här meddelandet. Så här granskar du principerna:

1. Gå Microsoft 365 Defender principer för samarbete & e-post och & principer för hot mot skräppost i avsnittet Principer i <https://security.microsoft.com/>  \>  \>  \> webbportalen **för** **e-Microsoft 365 Defender.**

   Om du vill gå direkt till sidan **Principer för skräppostskydd** använder du <https://security.microsoft.com/antispam>.

2. På sidan Principer för skydd mot skräppost markerar du principen genom att klicka på namnet på principen **(Typ** är **Custom anti-spam** policy eller **Name** is **Anti-Spam inbound policy (Default)**). 
3. I den utfällade informationen som visas väljer **du Redigera** åtgärder i **avsnittet** Åtgärder.
4. I avsnittet **Meddelandeåtgärder** granskar du omdömena **för skräppost,** skräppost  med hög konfidens, nätfiske och nätfiske med hög konfidens för att se om något av följande värden är markerat:  
   - **Lägg till X-sidhuvud**
   - **Förbereda ämnesraden med text**
   - **Omdirigera meddelandet till e-postadress**
   - **Ta bort meddelande**
   - **Ingen åtgärd**

   Det är möjligt att **standardinställningarna som tillämpats** på alla Exchange Online Protection påverkade meddelandet.

Mer information finns i [Konfigurera principer för skräppostskydd i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
