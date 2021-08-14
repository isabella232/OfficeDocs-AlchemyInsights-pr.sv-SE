---
title: Adresser Teams inloggningsfel AADSTS9000411
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
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953059"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Adresser Teams inloggningsfel AADSTS9000411

När du loggar in på Microsoft Teams kan du få felmeddelandet: Tyvärr har vi problem med att logga in dig i **AADSTS9000411: Begäran är inte korrekt formaterad. Parametern "login_hint" dupliceras.**

Åtgärda problemet genom att se till att Microsoft Teams klienterna har uppdaterats. Mer information om hur du uppdaterar klienten finns [i Uppdatera Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Om du av någon anledning inte kan uppdatera klienten rensas de flesta cachelagrade data när du loggar ut från klienten. Om du fortfarande har problem efter inloggning/inloggning avslutar du Teams och rensar klientcachen genom att göra följande:
1. Stäng Microsoft Teams.
2. Gå till: %appdata%\microsoft\teams och ta bort alla filer.
3. Öppna Microsoft Teams.
