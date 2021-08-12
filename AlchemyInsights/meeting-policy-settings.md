---
title: Inställningar för mötesprincip
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925183"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Hantera mötesprinciper i Microsoft Teams

**Obs! Det kan ta upp till 24 timmar innan principändringarna verkställs för användarna.** Du kanske inte kan ändra nyligen skapade principer direkt. vänta 4 timmar och försök sedan ändra en princip som nyligen skapats igen.

Mötesprinciper används för att styra vilka funktioner som är tillgängliga för mötesdeltagare för möten som schemaläggs av användare i organisationen. Vissa funktioner i mötes principer kanske inte implementeras i Teams administrationscenter ännu (dessa heter "kommer snart" i dokumentationen). I det här fallet, eller om du får ett felmeddelande som "Det går inte att uppdatera principen just nu men försök igen senare" i administrationscentret för Microsoft Teams, rekommenderar vi att du använder PowerShell för att skapa eller ändra Teams mötes principer. 

Mer information om mötesprinciper finns i följande resurser:

- Mer information om hur du skapar principer, ändrar och tilldelar användare till principen finns i [Hantera mötesprinciper i Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Information om hur du gör principändringar med PowerShell-cmdlets finns [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Du måste använda [PowerShell-Skype för företag-modulen för](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams-mötesprinciper. 
    - Mer information [finns i dokumentationen för *-CsTeamsMeetingPolicy-cmdlets.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

