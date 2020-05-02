---
title: Privat kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005456"
---
# <a name="private-channels-in-microsoft-teams"></a>Privata kanaler i Microsoft Teams

Privata kanaler är en ny funktion i Microsoft Teams. Observera att privata kanaler inte kan konverteras från standardkanaler eller vice versa.

Mer information om privata kanaler, till exempel information om [skapande och medlemskap](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) för privata kanaler och [sharepoint-webbplatser för privata kanaler,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)finns [i Privata kanaler i Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Anm.:** Eftersom konfiguration för bevarande av privata kanalmeddelanden ännu inte stöds, har klienter med bevarandeprinciper aktiverade inte privata kanaler aktiverade som standard. Privata kanaler kan aktiveras i administrationscentret för Teams. Observera också att även om lagring av privata kanalmeddelanden inte stöds, stöds lagring av filer som delas i privata kanaler.

**Behöver du en ny teamägare?**

Om din privata kanalägare lämnar kan du lägga till en ny gruppägare via Teams Powershell.


- Gå [hit](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) för att installera Teams Powershell.

Här är cmdlet du behöver:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Mer information om Teams Powershell finns i [Teams PowerShell Översikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
