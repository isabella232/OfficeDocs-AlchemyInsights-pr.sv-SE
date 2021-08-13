---
title: Kommentarer för listobjekt
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
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995525"
---
# <a name="comments-on-list-items"></a>Kommentarer för listobjekt

Användarna kan visa alla kommentarer för ett listobjekt och filtrera mellan vyer som visar kommentarer eller aktiviteter relaterade till ett objekt.

Användarna måste notera följande innan de kan lägga till och ta bort kommentarer:

- Kommentarer följer de behörighetsinställningar som är SharePoint.
- Klassiska listor som ännu inte är byggda för att visas i moderna användargränssnitt, till exempel uppgiftslistor, har inte den här kommentarsfunktionen.
- Kommentarer för listor i Teams inte tillgänglig i den här versionen.
- Kommentarer indexeras inte av Sök.

Administratörer kan inaktivera den här funktionen på organisationsnivå genom att ändra parametern **CommentsOnListItemsDisabled** i **PowerShell-cmdleten Set-SPOTenant.**

Det går för närvarande inte att inaktivera kommentarer på webbplats- eller listnivå. Vi hoppas att de kontrollerna finns i en senare uppdatering, förmodligen under det första kvartalet 2021.
