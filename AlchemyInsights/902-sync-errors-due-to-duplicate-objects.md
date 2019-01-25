---
title: 902 (synkroniseringsfel på Duplicera objekt)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492765"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniseringsfel på Duplicera objekt

Du kan få något av följande felmeddelanden visas när directory-synkroniseringen är klar:
  
- Det gick inte att uppdatera det här objektet i Microsoft Online Services eftersom följande attribut som associeras med det här objektet har värden som redan kan vara kopplad till ett annat objekt i den lokala katalogen.
    
- Det finns redan ett synkroniserat objekt med samma proxyadress i Microsoft Online Services-katalogen.
    
- Det gick inte att uppdatera det här objektet eftersom följande attribut som associeras med det här objektet har värden som redan kan vara kopplad till ett annat objekt i din lokala katalogtjänster: UserPrincipalName.
    
Hämta och kör [IdFix DirSync fel reparation verktyg](https://www.microsoft.com/download/details.aspx?id=36832)för att identifiera och åtgärda problemet.
  
Mer information finns i [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
  

