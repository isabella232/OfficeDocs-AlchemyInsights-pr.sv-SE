---
title: Microsoft Teams-gäst åtkomst
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: da9ecca062bd5f1dcc169657483ba53eb201def0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798394"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams-gäst åtkomst

Om du behöver hjälp med att kommunicera med användare utanför organisationen i Teams måste du bestämma om du ska använda [gäst åtkomst eller extern åtkomst (Federation)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)eller båda.

Kontrol lera [skillnaderna](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) för att förstå vilka funktioner som finns tillgängliga för dem.  Extern åtkomst (Federation) tillåter till exempel att 1:1 kommunikation, som chatt och närvaro.  Externa användare kan inte delta i samarbetet för Teams.  Om du vill att en extern användare ska delta i och delta i Teams kanal konversationer eller dela filer måste du aktivera gäst åtkomst.

**Alternativ 1: Aktivera gäst åtkomst**   
I administrations centret för team går du till [organisationens inställningar > gäst åtkomst](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) och aktiverar "Tillåt gäst åtkomst i Teams".  För en innehavare med alla andra standardinställningar bör detta vara allt du behöver göra.  Om du vill anpassa din gäst konfiguration kontrollerar du att du följer alla steg i [Check listan för gäst åtkomst](https://docs.microsoft.com/microsoftteams/guest-access-checklist). När du är klar måste du [vänta upp till 24 timmar](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) innan inställningarna börjar gälla.

Om du är säker på att du har slutfört alla stegen i check listan och det är mer än 24 timmar, kan du försöka [lägga till en gäst i gruppen](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Mer information om hur du gör videoklipp finns i [gäst åtkomst i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Alternativ 2: Aktivera extern åtkomst (Federation)** Om du även vill aktivera extern åtkomst (Federation) i administrations centret för team går du till inställningar för [hela organisationen > extern åtkomst](https://admin.teams.microsoft.com/company-wide-settings/external-communications) och aktiverar "användare kan kommunicera med Skype för företag och Teams", och följer sedan alla steg i [låta dina team användare chatta och kommunicera med användare i en annan organisation](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).


