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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724172"
---
# <a name="comments-on-list-items"></a>Kommentarer om List objekt

Användare kan visa alla kommentarer på ett List objekt och filtrera mellan vyer som visar kommentarer eller aktiviteter relaterade till ett objekt.

Användare måste anteckna följande innan de kan lägga till och ta bort kommentarer:

- Kommentarer följer de behörighets inställningar som finns i SharePoint.
- Klassiska listor som ännu inte har byggts för att visas i moderna användar gränssnitt, som aktivitets listor, har inte den här kommentars funktionen.
- Det går inte att kommentera listor i Teams med den här versionen.
- Kommentarer indexeras inte efter sökning.

Administratörer kan inaktivera den här funktionen på organisations nivå genom att ändra parametern **CommentsOnListItemsDisabled** i PowerShell-cmdleten **Set-SPOTenant** .

Det går för närvarande inte att inaktivera kommentarer på webbplats-eller listnivå. Vi hoppas att få dessa kontroller i en senare uppdatering, troligen i det första kvartalet 2021.
