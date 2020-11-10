---
title: Kommentarer om List objekt
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982556"
---
# <a name="comments-on-list-items"></a>Kommentarer om List objekt

Användarna kan snart lägga till och ta bort kommentarer för List objekt. Användare kan visa alla kommentarer på ett List objekt och filtrera mellan vyer som visar kommentarer eller aktiviteter relaterade till ett objekt.

**Tids inställning** :

**Riktad version** : successivt utgiven i Mid-oktober och förväntas bli färdig med Mid-november

**Standard version** : successivt utgiven i Mid-november och förväntas bli slutfört av tidigt december

**Rollout** Installation: riktad version för hela organisationen

Användare måste anteckna följande innan de kan lägga till och ta bort kommentarer:

- Kommentarer följer de behörighets inställningar som finns i SharePoint.
- Klassiska listor som ännu inte har byggts för att visas i moderna användar gränssnitt, som aktivitets listor, har inte den här kommentars funktionen.
- Det går inte att kommentera listor i Teams med den här versionen.
- Kommentarer indexeras inte efter sökning.

Administratörer kan inaktivera den här funktionen på organisations nivå genom att ändra parametern **CommentsOnListItemsDisabled** i PowerShell-cmdleten **Set-SPOTenant** .

Det går för närvarande inte att inaktivera kommentarer på webbplats-eller listnivå. Vi hoppas att få dessa kontroller i en senare uppdatering, troligen i det första kvartalet 2021.
