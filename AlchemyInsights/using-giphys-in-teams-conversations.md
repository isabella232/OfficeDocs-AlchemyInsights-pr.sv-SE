---
title: Använda Giphys i Teams konversationer
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323538"
---
# <a name="using-giphys-in-teams-conversations"></a>Använda Giphys i Teams konversationer

Giphys åtkomst i Teams chatt är aktiverad som standard. Som administratör kan du styra om Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) är tillgänglig för användare genom att ange en meddelandeprincip och se till att Använd **Giphys** i konversationer **är På.**

Om GIF-filer inte fungerar som förväntat i Teams konversationer kontrollerar du följande:

[Meddelandeprincipen](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) måste tillåta Giphys. Så här verifierar du med hjälp av PowerShell-cmdlets:

- Kontrollera att du kan [hantera Teams med PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Kör [PowerShell-kommandot Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) och kontrollera att **AllowGiphy** är inställt på **SANT.**
- Om **AllowGiphy** är inställt på **FALSKT** kör du följande [PowerShell-kommando Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Valfri anslutna upplevelser](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) måste aktiveras för att tillåta åtkomst till GIPHY URL.

**Obs!** Om du har flera Teams Messaging-principer konfigurerade för klientorganisationen kan du fastställa identiteten för principen som tilldelats den påverkade användaren med [PowerShell-kommandot Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Välj TeamsMessagingPolicy.
