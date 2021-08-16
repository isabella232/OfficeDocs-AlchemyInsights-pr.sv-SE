---
title: Om Yammer administratörer
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
ms.openlocfilehash: a5d71f509b7006264b15549c7e8450d4ed7025b7dea3cfd80fe6f0fdf50b0b9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989737"
---
# <a name="about-yammer-admins"></a>Om Yammer administratörer

**Nätverksadministratörer**

Globala administratörer framhävs automatiskt till rollen Verifierad administratör i ett Yammer nätverk. I följande fall kan den här kampanjen inte ske på rätt sätt:

- Flera Yammer nätverk finns och administratören loggas in på fel nätverk. [Nätverkskonsolidering](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) krävs för att komma till ett Yammer nätverk.
- Azure PIM används. Användaren kanske inte är global administratör tillräckligt länge för att kampanjen ska kunna ske. En kommande uppdatering av Yammer kan lösa problemet, men det är bäst att ge användarna en global administratör manuellt.
- Det finns ett synkroniseringsproblem med Yammer nätverk. I det här fallet krävs en supportbegäran för ytterligare undersökning.

Mer information om hur Yammer administratörsroller finns [i Hantera Yammer administratörer.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)

**Gruppadministratörer**

Gruppadministratörer för Microsoft 365-anslutna grupper synkroniseras med gruppmedlemskap från Azure AD. För stora grupper kan synkroniseringen ta en längre tid.
