---
title: Om Yammer-administratörer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038126"
---
# <a name="about-yammer-admins"></a>Om Yammer-administratörer

**Nätverksadministratörer**

Globala administratörer framhävs automatiskt till rollen verifierad administratör i ett Yammer-nätverk. I följande fall kan den här kampanjen inte ske på rätt sätt:

- Det finns flera Yammer-nätverk och administratören loggas in på fel nätverk. [Nätverkskonsolidering](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) krävs för att komma till ett Yammer-nätverk.
- Azure PIM används. Användaren kanske inte är global administratör tillräckligt länge för att kampanjen ska kunna ske. En kommande uppdatering av Yammer kan lösa problemet, men det är bäst att göra användarna till globala administratörer manuellt.
- Det finns ett synkroniseringsproblem med Yammer-nätverket. I det här fallet krävs en supportbegäran för ytterligare undersökning.

Mer information om administratörsroller i Yammer finns [i Hantera Yammer-administratörer.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)

**Gruppadministratörer**

Gruppadministratörer för Microsoft 365-anslutna grupper synkroniseras med gruppmedlemskap från Azure AD. För stora grupper kan synkroniseringen ta en längre tid.
