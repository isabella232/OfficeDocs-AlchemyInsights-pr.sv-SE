---
title: Adressering av Inloggningsfel i Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822005"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adressering av Inloggningsfel i Teams AADSTS9000411

När du loggar in i Microsoft Teams kan du få felmeddelandet: Tyvärr, men vi har problem med att logga in dig i **AADSTS9000411: Begäran är inte korrekt formaterad. Parametern "login_hint" dupliceras.**

Åtgärda problemet genom att se till att dina Microsoft Teams-klienter är uppdaterade. Mer information om hur du uppdaterar din klient finns [i Uppdatera Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Om du av någon anledning inte kan uppdatera klienten rensas de flesta cachelagrade data när du loggar ut från klienten. Avsluta Teams om du fortfarande har problem efter inloggning/inloggning och rensa klientcachen genom att göra följande:
1. Stäng Microsoft Teams.
2. Gå till: %appdata%\microsoft\teams och ta bort alla filer.
3. Öppna Microsoft Teams igen.
