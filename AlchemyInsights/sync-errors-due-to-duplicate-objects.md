---
title: 902 (synkroniseringsfel på grund av dubblettobjekt)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998818"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniseringsfel på grund av duplicerade objekt

Du kan få något av följande felmeddelanden när katalogsynkroniseringen är klar Microsoft 365:

- Det går inte att uppdatera objektet i Microsoft Online Services eftersom följande attribut som är kopplade till det här objektet har värden som kanske redan är kopplade till ett annat objekt i din lokala katalog.

- Det finns redan ett synkroniserat objekt med samma proxyadress i din Microsoft Online Services-katalog.

- Det går inte att uppdatera det här objektet eftersom följande attribut som är kopplade till det här objektet har värden som kanske redan är kopplade till ett annat objekt i dina lokala katalogtjänster: UserPrincipalName.

Identifiera och åtgärda problemet genom att ladda ned och köra [felreparationsverktyget IdFix DirSync.](https://github.com/Microsoft/idfix)

Mer information finns i [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
