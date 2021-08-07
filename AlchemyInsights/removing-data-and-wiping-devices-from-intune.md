---
title: Tar bort data och rensar enheter från Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922280"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Tar bort data och rensar enheter från Intune

Fjärråtgärderna Ta enhet ur bruk och Rensa enhet kan användas för att ta bort företagsdata som hanteras av Intune, eller för att utföra en fabriksåterställning och återställa enheten till dess standardinställningar.

1. Logga in på Microsoft 365 Enhetshantering och fortsätt till **Enheter** > **Alla enheter**.
2. Välj den enhet du vill rensa.
3. Välj den typ av fjärrensning du vill göra. Ta ur bruk tar endast bort organisationsinformation, medan en hel rensning återställer enheten till fabriksinställningarna.
4. Bekräfta genom att välja **Ja**. Tills rensningen är klar visas enhetsåtgärdsstatusen som *Ta ur bruk pågående*.
    När åtgärden har slutförts visas inte längre den mobila enheten i listan över hanterade enheter.

> [!NOTE]
> Företagsdata kan inte tas bort från enheter som är anslutna till Azure AD. 

Fullständig information om effekterna av åtgärderna Ta ur bruk och Rensa, inklusive vad som behålls och vad som tas bort, finns i följande dokumentation:

- [Ta bort enheter genom att rensa, ta ur bruk eller avregistrera enheten manuellt](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Så här rensar du endast företagsdata från appar som hanteras av Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Radera alla data från macOS-enheter](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).