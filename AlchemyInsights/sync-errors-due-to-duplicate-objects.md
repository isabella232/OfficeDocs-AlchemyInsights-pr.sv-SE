---
title: 902 (Synkroniseringsfel på grund av dubblettobjekt)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767157"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniseringsfel på grund av dubblettobjekt

Ett av följande felmeddelanden kan visas när katalogsynkroniseringen är klar i Microsoft 365:

- Det går inte att uppdatera objektet i Microsoft Online Services eftersom följande attribut som är associerade med det här objektet har värden som kanske redan är associerade med ett annat objekt i den lokala katalogen.

- Det finns redan ett synkroniserat objekt med samma proxyadress i microsoft onlinetjänstkatalogen.

- Det går inte att uppdatera det här objektet eftersom följande attribut som är associerade med det här objektet har värden som kanske redan är associerade med ett annat objekt i dina lokala katalogtjänster: UserPrincipalName.

Om du vill identifiera och åtgärda problemet hämtar och kör [du IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).

Mer information finns i [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
