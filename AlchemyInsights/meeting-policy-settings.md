---
title: Inställningar för Mötes princip
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
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794352"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Hantera Mötes principer i Microsoft Teams

**Obs! det kan ta upp till 24 timmar innan princip ändringarna börjar gälla för användarna.** Du kanske inte kan göra ändringar i nyskapade principer omedelbart; vänta 4 timmar och försök sedan att ändra en nyligen skapad princip igen.

Mötes principer används för att kontrol lera vilka funktioner som är tillgängliga för Mötes deltagare för möten som har schemalagts av användare i organisationen. Vissa funktioner för Mötes principer kanske inte implementeras i team administrations centret ännu (de här är märkta "kommer snart" i dokumentationen). I det här fallet, eller om du får ett fel meddelande som "vi kan inte uppdatera policyn just nu, men prova igen senare" i administrations centret för Microsoft Teams rekommenderar vi att du använder PowerShell för att skapa eller ändra principer för team möten. 

Mer information om Mötes principer finns i följande resurser:

- Information om hur du skapar principer, gör ändringar och tilldelar användare till principer finns i [Hantera Mötes principer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Information om hur du ändrar princip ändringar med PowerShell-cmdletar finns i [Översikt över Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Du måste använda PowerShell- [modulen i Skype för företag](https://www.microsoft.com/download/details.aspx?id=39366) för att få arbets grupper. 
    - Läs [dokumentationen för *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) för mer information.

