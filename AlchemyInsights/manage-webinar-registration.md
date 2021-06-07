---
title: Hantera registrering för webbsswebb
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794145"
---
# <a name="manage-webinar-registration"></a>Hantera registrering för webbsswebb

Du hanterar vem som kan registrera sig för Teams-webbssyssor med hjälp Teams Powershell-kommandon. Information om hur du Teams Powershell finns [i Teams PowerShell.](/microsoftteams/teams-powershell-install) 

*WhoCanRegister är aktiverat och* inställt på **EveryoneInCompany som standard.** Om du vill tillåta att alla, även anonyma användare, registrerar sig måste du ställa in mötespolicyn på **Alla** med powershell-kommandot:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Obs!** Om anonym anslutning har inaktiverats i mötesinställningarna kan anonyma användare inte ansluta till webbss webbseningar. Mer information och hur du aktiverar den här inställningen finns [i Hantera mötesinställningar i Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Om du vill inaktivera mötesregistrering anger du *AllowMeetingRegistration till* **False**.

Mer information om hur du konfigurerar vem som kan registrera sig för webbsenter finns i [Konfigurera vem som kan registrera sig för webbssalar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Mer information om inställningar för Microsoft-listor finns i [Kontrollinställningar för Microsoft-listor.](/sharepoint/control-lists)
