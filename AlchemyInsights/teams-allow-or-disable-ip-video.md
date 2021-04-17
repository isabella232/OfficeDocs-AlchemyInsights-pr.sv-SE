---
title: Teams tillåta eller inaktivera IP-video
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826361"
---
# <a name="teams-allow-or-disable-ip-video"></a>Teams tillåta eller inaktivera IP-video

**Ändra eller skapa en mötesprincip**

Om du vill ändra eller skapa en mötesprincip går du till **administrationscentret** för Microsoft Teams > möten > mötes principer . Välj en princip från listan eller klicka på **Lägg till**. Om du skapar en ny princip kan du lägga till ett namn och en beskrivning. Namnet får inte innehålla specialtecken eller vara längre än 64 tecken. Välj önskade inställningar och klicka på **OK**.

Säg till exempel att du har många användare och du vill begränsa den mängd bandbredd som skulle krävas för deras möte. Du kan skapa en ny anpassad princip med namnet "Begränsad bandbredd" och inaktivera följande inställningar:

Under **Ljud och video**:

- Inaktivera Tillåt molninspelning.
- Inaktivera Tillåt IP-video.

Tilldela sedan principen till användarna.

**Tilldela en mötespolicy till användare**

1. I den vänstra navigeringen i administrationscentret för Microsoft Teams går du till **Användare** och klicka sedan på användaren.
2. Markera användaren genom att klicka till vänster om användarnamnet och sedan klicka på **Redigera inställningar**.
3. Under **Mötesprincip** väljer du den princip du vill tilldela och klickar sedan på **Använd.**

Mer information finns i Hantera [mötesprinciper i Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)
