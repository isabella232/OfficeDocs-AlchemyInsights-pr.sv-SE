---
title: Dynamics 365 - fel instrumentpanelen visas i Dynamics 365 enhetligt gränssnitt
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528569"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Fel instrumentpanelen visas i Dynamics 365 enhetligt gränssnitt

Det finns flera orsaker till varför du kan se en annan instrumentpanel än förväntat:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Användaren har angett en standard 

Vanligtvis kan du identifiera en användare standardinstrumentpanel anges om knappen **Ange som standard** inte visas i kommandofältet instrumentpanelen. Användaren standardinstrumentpanel åsidosätts alla standard-instrumentpaneler även om användarinstrumentpanel standard inte är den aktuella appen.

Använd följande lösning ta bort deras standardinstrumentpanel.

1. Skapa en ny personlig instrumentpanel.

2. Ange den nya instrumentpanelen som standard.

3. Ta bort den här instrumentpanelen.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Instrumentpanelen är inställd i Webbplatsöversikt

Du kan ha angett en standardinstrumentpanel för organisationen genom att välja en instrumentpanel och välja 'Ange som standard ”under” Anpassa systemet ”. Men instrumentpanelen som definierats i sitemap designer har högre prioritet än den här instrumentpanelen om användaren har åtkomst till den.

Om du vill att användare kan visa på instrumentpanelen som du angett som Organisationsstandard, kan du antingen:

* Ange att instrumentpanelen i Webbplatsöversikt

* Ta bort åtkomst till instrumentpanelen sitemap definieras för dessa användare
