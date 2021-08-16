---
title: Microsoft Teams – gäståtkomst
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
ms.openlocfilehash: 2c78fec14d43c5cbf6aebbc889d606eb2f6c4c64af85997f523d06872c911a0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012326"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams – gäståtkomst

Om du behöver hjälp med att kommunicera med användare utanför organisationen i Teams måste du bestämma om du ska använda gäståtkomst eller extern åtkomst [(federation)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)eller båda.

Se till att [granska skillnaderna för att](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) förstå de tillgängliga funktionerna för var och en.  Till exempel tillåter extern åtkomst (federation) 1:1-kommunikation, t.ex. chatt och närvaro.  Externa användare kan dock inte delta i Teams samarbete.  Om du vill att en extern användare ska kunna delta i Teams-kanalkonversationer eller Dela filer måste du aktivera gäståtkomst.

**Alternativ 1: Aktivera gäståtkomst** Gå Teams organisationsomfattande gäståtkomst [i administrationscentret för Inställningar > och](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) aktivera Tillåt gäståtkomst i Teams.  För en klientorganisation med alla andra standardinställningar ska det vara allt du behöver göra.  Anpassa konfigurationen av gäståtkomst genom att kontrollera att du följer alla steg i checklistan [för gäståtkomst.](https://docs.microsoft.com/microsoftteams/guest-access-checklist) När du är klar måste du vänta i [upp till 24](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) timmar på att inställningarna börjar gälla.

Om du är säker på att du har slutfört alla steg i checklistan och det har gått mer än 24 timmar kan du försöka lägga till en gäst i [teamet.](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop)

Mer information, inklusive videofilmer, finns i [Gäståtkomst i Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Alternativ 2: Aktivera extern åtkomst (federation)** Om du även vill aktivera extern åtkomst (federation) går du till Organisationsomfattande administrationscenter för Teams Inställningar > extern åtkomst och aktiverar "Användare kan kommunicera med Skype för företag- och Teams-användare" och följer sedan anvisningarna i Låta [Teams-användarna](https://admin.teams.microsoft.com/company-wide-settings/external-communications) chatta och kommunicera med användare i en [annan](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)organisation.
