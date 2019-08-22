---
title: 902 (synkroniseringsfel på Duplicera objekt)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507433"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniseringsfel på Duplicera objekt

Du kan få något av följande felmeddelanden visas när katalogsynkronisering i Office 365:

- Det gick inte att uppdatera det här objektet i Microsoft Online Services eftersom följande attribut som associeras med det här objektet har värden som redan kan vara kopplad till ett annat objekt i den lokala katalogen.

- Det finns redan ett synkroniserat objekt med samma proxyadress i Microsoft Online Services-katalogen.

- Det gick inte att uppdatera det här objektet eftersom följande attribut som associeras med det här objektet har värden som redan kan vara kopplad till ett annat objekt i din lokala katalogtjänster: UserPrincipalName.

Hämta och kör [IdFix DirSync fel reparation verktyg](https://www.microsoft.com/download/details.aspx?id=36832)för att identifiera och åtgärda problemet.

Mer information finns i [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
