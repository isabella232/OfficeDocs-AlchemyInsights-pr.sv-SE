---
title: Dynamics 365-fel instrumentpanel visas i Dynamics 365 enhetligt gränssnitt
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528569"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Fel instrumentpanel visas i Dynamics 365 enhetligt gränssnitt

Det finns flera anledningar till att du kan se en annan instrumentpanel än den du förväntar dig:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Användaren har angett en standardinstrumentpanel för användare 

Vanligtvis kan du identifiera en standardinstrumentpanel för användare anges om knappen **Ange som standard** inte visas i instrumentpanelens kommandofält. Standardinstrumentpanelen för användare åsidosätter alla andra standardinstrumentpaneler, även om användarens standardinstrumentpanel inte finns i den aktuella appen.

Använd följande lösning för att ta bort deras standardinstrumentpanel.

1. Skapa en ny personlig instrumentpanel.

2. Ange den nya instrumentpanelen som Användarstandard.

3. Ta bort den instrumentpanelen.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Instrumentpanelen anges i webbplatsöversikten

Du kan ha ställt in en standardinstrumentpanel för organisationen genom att välja en instrumentpanel och välja "Ange som standard" under "anpassa systemet". Men instrumentpanelen som definierats i sitemap-designern kommer att ha företräde framför den här instrumentpanelen, om användaren har åtkomst till den.

Om du vill att användarna ska se den instrumentpanel som du har angett som standard för organisationen kan du antingen:

* Ange den instrumentpanelen i webbplatsöversikten

* Ta bort åtkomsten till webbplatsöversikten definierad instrumentpanel för dessa användare
