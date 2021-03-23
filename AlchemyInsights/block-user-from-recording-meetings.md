---
title: Blockera användare från att spela in möten
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037067"
---
# <a name="block-user-from-recording-meetings"></a>Blockera användare från att spela in möten

Om du behöver förhindra **eller blockera specifika användare** från att spela in Teams-möten kan du göra det via inställningar för Teams mötespolicy. I administrationscentret för Microsoft Teams inaktiverar du inställningen **Tillåt molninspelning** i den mötesprincip som tilldelats den användaren. Mer information finns i [Hantera mötesprinciper i Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)

Använd supportdiagnostik för att verifiera om en viss användare tillåts eller inte kan spela in Teams-möten. Kör en ny supportfråga och skriv i **Diag: Mötesinspelning** – diagnostiken kontrollerar principinställningarna för den angivna användaren och bestämmer principinställningarna. Tänk på att det kan ta några timmar innan de nya principinställningarna börjar gälla, så om du precis har gjort en ändring bör du vänta några timmar innan du kör diagnostiken igen.

Mer information finns i [Aktivera eller inaktivera molninspelning.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
