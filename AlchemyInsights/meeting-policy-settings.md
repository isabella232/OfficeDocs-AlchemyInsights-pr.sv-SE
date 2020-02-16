---
title: Inställningar för mötesprincip
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042862"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Hantera mötesprinciper i Microsoft Teams

**Det kan ta upp till 24 timmar innan principändringar träder i kraft för användarna.** Du kanske inte kan göra ändringar i nyskapade principer omedelbart. vänta 4 timmar och försöka ändra en nyskapad princip igen.

Mötesprinciper används för att styra de funktioner som är tillgängliga för mötesdeltagare för möten som schemaläggs av användare i organisationen. Vissa funktioner i mötesprinciper kanske inte implementeras i administrationscentret teams ännu (dessa är märkta "kommer snart" i dokumentationen). I det här fallet, eller om du får ett felmeddelande som "Vi kan inte uppdatera principen just nu men prova den igen senare" i administrationscentret för Microsoft Teams rekommenderar vi att du använder PowerShell för att skapa eller ändra teams mötesprinciper. 

Mer information om mötesprinciper finns i följande resurser:

- Mer information om hur du skapar principer, gör ändringar och tilldela användare till principen finns i [Hantera mötesprinciper i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Mer göra principändringar med PowerShell-cmdlets finns i [Team PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Du måste använda [Skype för företag PowerShell-modulen](https://www.microsoft.com/download/details.aspx?id=39366) för teams mötesprinciper. 
    - Läs [dokumentationen *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) för mer information.

