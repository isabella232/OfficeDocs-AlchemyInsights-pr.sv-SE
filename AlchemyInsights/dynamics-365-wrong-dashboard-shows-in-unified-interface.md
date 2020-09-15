---
title: Dynamics 365 – fel instrument panel visas i Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711293"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Fel instrument paneler i det enhetliga gränssnittet för Dynamics 365

Det finns flera orsaker till att du kan se en annan instrument panel än den du förväntar dig:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Användaren har ställt in en standard instrument panel för användare 

Vanligt vis kan du identifiera en standard instrument panel för användare om knappen **Ange som standard** inte visas i instrument panels kommando fältet. Standard instrument panelen för användare åsidosätter alla andra standard instrument paneler, även om användarens standard instrument panel inte finns i den aktuella appen.

Använd följande lösning för att ta bort standard instrument panelen.

1. Skapa en ny personlig instrument panel.

2. Ange att den nya instrument panelen ska vara standard.

3. Ta bort den instrument panelen.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Instrument panelen är inställd i sitemap

Du kan ha ställt in en standard instrument panel för organisationen genom att välja en instrument panel och välja "Ange som standard" under Anpassa systemet. Men instrument panelen som definierats i sitemap-fönstret har högre prioritet än den här instrument panelen, om användaren har åtkomst till den.

Om du vill att användarna ska kunna se den instrument panel du angett som standard organisation kan du antingen:

* Ange instrument panelen i sitemap

* Ta bort åtkomst till webbplats översikts instrument panelen för dessa användare
