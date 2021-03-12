---
title: Inställningar för mötesprincip
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704624"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Hantera mötesprinciper i Microsoft Teams

**Obs! Det kan ta upp till 24 timmar innan principändringarna verkställs för användarna.** Du kanske inte kan ändra nyligen skapade principer omedelbart. Vänta 4 timmar och försök sedan ändra en ny princip igen.

Mötesprinciper används för att styra vilka funktioner som är tillgängliga för mötesdeltagare för möten som schemaläggs av användare i organisationen. Vissa funktioner i mötes principer kanske inte implementeras i administrationscentret för Teams ännu (dessa märks "kommer snart" i dokumentationen). I det här fallet, eller om du får ett felmeddelande som "Vi kan inte uppdatera principen just nu men försök igen senare" i administrationscentret för Microsoft Teams rekommenderar vi att du använder PowerShell för att skapa eller ändra mötespolicyer för Teams. 

Mer information om mötesprinciper finns i följande resurser:

- Mer information om hur du skapar principer, gör ändringar och tilldelar användare till principen finns i [Hantera mötesprinciper i Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Information om hur du gör principändringar med PowerShell-cmdlets [finns i Översikt över Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Du måste använda Skype för [företag PowerShell-modulen för](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams-mötesprinciper. 
    - Mer information finns i dokumentationen [för *-CsTeamsMeetingPolicy-cmdlets.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

