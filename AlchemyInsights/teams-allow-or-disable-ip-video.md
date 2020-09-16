---
title: Teams Tillåt eller inaktivera IP-video
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670202"
---
# <a name="teams-allow-or-disable-ip-video"></a>Teams Tillåt eller inaktivera IP-video

**Ändra eller skapa en Mötes princip**

Om du vill ändra eller skapa en Mötes princip går du till **administrations centret för Microsoft team >-möten > Mötes principer**. Välj en princip från listan eller klicka på **Lägg till**. Om du skapar en ny princip kan du lägga till ett namn och en beskrivning. Namnet får inte innehålla specialtecken eller vara längre än 64 tecken. Välj önskade inställningar och klicka på **OK**.

Säg till exempel att du har många användare och vill begränsa hur mycket bandbredd som ska krävas för mötet. Du kan skapa en ny anpassad princip med namnet "Begränsad bandbredd" och inaktivera följande inställningar:

Under **Ljud och video**:

- Inaktivera Tillåt molninspelning.
- Inaktivera Tillåt IP-video.

Tilldela sedan principen till användarna.

**Tilldela en mötespolicy till användare**

1. I den vänstra navigeringen i administrationscentret för Microsoft Teams går du till **Användare**och klicka sedan på användaren.
2. Markera användaren genom att klicka till vänster om användarnamnet och sedan klicka på **Redigera inställningar**.
3. Under **Mötes princip**väljer du den princip som du vill tilldela och klickar sedan på **Använd**.

Mer information finns i [Hantera Mötes principer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).
