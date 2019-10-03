---
title: Principinställningar för möten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376856"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Hantera Mötes principer i Microsoft Teams

Mötes principer används för att styra de funktioner som är tillgängliga för mötesdeltagare för möten som schemaläggs av användare i din organisation. Vissa funktioner i Mötes principer kanske inte implementeras i Teams administratörscenter ännu (dessa är märkta "kommer snart" i dokumentationen). I det här fallet, eller om du får ett felmeddelande som "vi kan inte uppdatera principen just nu men försök igen senare" i Microsoft Teams administratörscenter, rekommenderar vi att du använder PowerShell för att skapa eller ändra Teams Mötes principer. 

Mer information om Mötes principer finns i följande resurser:

- Mer information om hur du skapar principer, gör ändringar och tilldelar användare till principen finns [i hantera Mötes principer i Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Om du vill göra principändringar med hjälp av PowerShell-cmdlets, se [Teams PowerShell-översikt](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Du måste använda [Skype för Business PowerShell-modulen](https://www.microsoft.com/download/details.aspx?id=39366) för team Mötes principer. 
    - Granska [dokumentationen för *-csteamsmeetingpolicy cmdlets](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) för mer information.

**Anmärkning:** Det kan ta upp till 24 timmar innan principändringarna träder i kraft för användarna. Du kanske inte kan göra ändringar i nyligen skapade principer omedelbart. vänta 4 timmar och försök att ändra en nyskapad princip igen. Om du fortfarande har problem kan du prova PowerShell.  