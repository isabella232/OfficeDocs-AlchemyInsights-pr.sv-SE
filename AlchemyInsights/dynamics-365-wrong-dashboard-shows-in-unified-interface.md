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
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748899"
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
