---
title: 902 (synkroniseringsfel på grund av dubbletter)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737359"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniseringsfel på grund av dubbletter av objekt

Du kan få något av följande fel meddelanden när profilsynkronisering slutar med Microsoft 365:

- Det går inte att uppdatera det här objektet i Microsoft Online Services eftersom följande attribut som är kopplade till det här objektet har värden som redan kan vara kopplade till ett annat objekt i din lokala katalog.

- Ett synkroniserat objekt med samma proxyadress finns redan i din Microsoft Online Services-katalog.

- Det går inte att uppdatera objektet eftersom följande attribut som är kopplade till det här objektet har värden som redan kan vara kopplade till ett annat objekt i din lokala katalog tjänst: UserPrincipalName.

Du kan identifiera och åtgärda problemet genom att hämta och köra [IdFix DirSync-verktyget](https://www.microsoft.com/download/details.aspx?id=36832).

Mer information finns i [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
