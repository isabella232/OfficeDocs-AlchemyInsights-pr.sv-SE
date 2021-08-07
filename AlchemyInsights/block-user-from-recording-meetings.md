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
ms.openlocfilehash: 7eb3fd34ec6f1a2d431ed276b00dd46b5ec6aa73d69b37ef88b1ba0ca6f5d077
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019202"
---
# <a name="block-user-from-recording-meetings"></a>Blockera användare från att spela in möten

Om du behöver förhindra **eller blockera specifika** användare från att Teams möten kan du göra det via Teams inställningar för mötesprincip. I Microsoft Teams i administrationscentret inaktiverar du **inställningen Tillåt molninspelning** i den mötesprincip som tilldelats den användaren. Mer information finns i [Hantera mötes principer i Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).

Om du vill verifiera om en viss användare tillåts eller inte kan spela Teams möten använder du supportdiagnostik. Kör en ny supportfråga och skriv i **Diag: Mötesinspelning** – diagnostiken kontrollerar principinställningarna för den angivna användaren och bestämmer principinställningarna. Tänk på att det kan ta några timmar innan de nya principinställningarna börjar gälla, så om du precis har gjort en ändring bör du vänta några timmar innan du kör diagnostiken igen.

Mer information finns i [Aktivera eller inaktivera molninspelning.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
