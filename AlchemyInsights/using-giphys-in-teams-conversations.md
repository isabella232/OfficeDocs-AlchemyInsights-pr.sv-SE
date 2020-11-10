---
title: Använda Giphys i Teams-konversationer
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
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982576"
---
# <a name="using-giphys-in-teams-conversations"></a>Använda Giphys i Teams-konversationer

Giphys Access in Teams-chatt är aktiverat som standard. Som administratör kan du kontrol lera om Giphys är tillgängliga för användare genom att [Ange en meddelande princip](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) och kontrol lera att **Använd Giphys i konversationer** är **aktiverat**.

Om GIF inte fungerar som förväntat i Teams-konversationer ska du kontrol lera:

[Meddelande princip](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) måste tillåta Giphys. Så här verifierar du med PowerShell-cmdletar:

- Kontrol lera att du kan [hantera team med PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Kör PowerShell-kommandot [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) och kontrol lera att **AllowGiphy** är inställt på **True**.
- Om **AllowGiphy** är inställt på **false** kör du följande PowerShell- [AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Valfri ansluten upplevelse](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) måste aktive ras för att tillåta åtkomst till GIPHY-URL: en.

> [!NOTE]
> Om du har flera team meddelande principer konfigurerade för din klient organisation kan du bestämma identiteten för den princip som tilldelats den påverkade användaren med PowerShell [-kommandot Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Välj TeamsMessagingPolicy.
