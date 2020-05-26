---
title: Åtgärda inloggningsfel för team AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358368"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Åtgärda inloggningsfel för team AADSTS9000411

När du loggar in på Microsoft Teams kan felet visas: **Tyvärr, men vi har problem med att logga in dig i AADSTS9000411: Begäran är inte korrekt formaterad. Parametern "login_hint" dupliceras.**

Om du vill lösa problemet bör du se till att dina Microsoft Teams-klienter är uppdaterade. Mer information om hur du uppdaterar klienten finns i [Uppdatera Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Om du inte kan uppdatera klienten av någon anledning rensas de flesta cachelagrade data genom att logga ut klienten. Men om du fortfarande har problem efter utloggning/inloggning avslutar du Teams och rensar klientcachen genom att göra följande:
1. Stäng Microsoft Teams.
2. Gå till: %appdata%\microsoft\teams och ta bort alla filer.
3. Öppna Microsoft Teams igen.
