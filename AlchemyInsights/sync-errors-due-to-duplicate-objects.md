---
title: 902 (Synkroniseringsfel på grund av dubbletter)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708080"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkroniseringsfel på grund av dubblettobjekt

Du kan få ett av följande felmeddelanden när katalogsynkroniseringen har avslutats i Microsoft 365:

- Det går inte att uppdatera objektet i Microsoft Online Services eftersom följande attribut som är kopplade till objektet har värden som kanske redan är associerade med ett annat objekt i din lokala katalog.

- Det finns redan ett synkroniserat objekt med samma proxyadress i din Microsoft Online Services-katalog.

- Det går inte att uppdatera objektet eftersom följande attribut som är kopplade till objektet har värden som redan kan vara kopplade till ett annat objekt i dina lokala katalogtjänster: UserPrincipalName.

Identifiera och åtgärda problemet genom att ladda ned och köra felreparationsverktyget [IdFix DirSync.](https://github.com/Microsoft/idfix)

Mer information finns i [KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
