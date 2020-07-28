---
title: Diagrammet visar olika antal poster i rutnätet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439961"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Diagrammet visar olika antal poster i rutnätet

**Symptom**

För diagram på instrumentpanelssidan, när du klickar på diagrammet "..." och klicka på "Visa poster", navigerar du till rutnätssidan för att se alla poster. Ibland ändras antalet poster.

**Orsak**

Detta beror på skillnaden mellan vyerna mellan diagrammet på den ursprungliga instrumentpanelssidan och diagrammet på rutnätets startsida.  

**Lösning**

1. Kontrollera vyn från den ursprungliga sidan och vyn i rutnätet för att se om de är annorlunda.
2. Ändra vyn i rutnätet så att den matchar vyn på den ursprungliga sidan.
3. Om rätt vy inte kan hittas betyder det vanligtvis att vyn inte är aktiverad i appdesignern.
4. Gå till appdesignern för den specifika appen, välj entiteten och dess vyer, kontrollera den vy som du vill aktivera, spara, publicera och stänga.
5. Uppdatera sidan.