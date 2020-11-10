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
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="9cb0b-102">Använda Giphys i Teams-konversationer</span><span class="sxs-lookup"><span data-stu-id="9cb0b-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="9cb0b-103">Giphys Access in Teams-chatt är aktiverat som standard.</span><span class="sxs-lookup"><span data-stu-id="9cb0b-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="9cb0b-104">Som administratör kan du kontrol lera om Giphys är tillgängliga för användare genom att [Ange en meddelande princip](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) och kontrol lera att **Använd Giphys i konversationer** är **aktiverat**.</span><span class="sxs-lookup"><span data-stu-id="9cb0b-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="9cb0b-105">Om GIF inte fungerar som förväntat i Teams-konversationer ska du kontrol lera:</span><span class="sxs-lookup"><span data-stu-id="9cb0b-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="9cb0b-106">[Meddelande princip](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) måste tillåta Giphys.</span><span class="sxs-lookup"><span data-stu-id="9cb0b-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="9cb0b-107">Så här verifierar du med PowerShell-cmdletar:</span><span class="sxs-lookup"><span data-stu-id="9cb0b-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="9cb0b-108">Kontrol lera att du kan [hantera team med PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="9cb0b-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="9cb0b-109">Kör PowerShell-kommandot [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) och kontrol lera att **AllowGiphy** är inställt på **True**.</span><span class="sxs-lookup"><span data-stu-id="9cb0b-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="9cb0b-110">Om **AllowGiphy** är inställt på **false** kör du följande PowerShell- [AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="9cb0b-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="9cb0b-111">[Valfri ansluten upplevelse](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) måste aktive ras för att tillåta åtkomst till GIPHY-URL: en.</span><span class="sxs-lookup"><span data-stu-id="9cb0b-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="9cb0b-112">Om du har flera team meddelande principer konfigurerade för din klient organisation kan du bestämma identiteten för den princip som tilldelats den påverkade användaren med PowerShell [-kommandot Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Välj TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="9cb0b-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
