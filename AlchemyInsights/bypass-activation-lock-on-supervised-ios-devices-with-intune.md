---
title: Kringgå aktiveringslås på övervakade iOS-enheter med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424211"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Kringgå aktiveringslås på övervakade iOS-enheter med Intune

Möjligheten att kringgå aktiveringslåset på iOS-enheter gör det enklare att återställa från scenariot där en användare aktiverar aktiveringslås på en företagsenhet och sedan lämnar företaget.

Förutsättningar för att kringgå ett aktiveringslås inkluderar:

- En enhet är som är "övervakad".
- Aktiveringslåset har aktiverats med hjälp av iOS-enhetsbegränsningsprincipen i Intune.

Dessutom, när du kringgår ett aktiveringslås, bör du:

- Fysiskt besitter enheten som torkas.
- Kopiera koden innan du utfärdar rensningen.

**Obs:** Rensningskoden är inte skiftlägeskänslig, så "-" tecknen krävs inte.

Mer information finns i [Kringgå aktiveringslås på övervakade iOS-enheter med Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**FAQ**

F: **Jag utfärdade en fjärråtgärd för att ta bort företagsdata från en enhet, och nu har den fastnat i ett väntande tillstånd.**

S: För att en fjärråtgärd ska kunna slutföras måste den riktade enheten vara online och felfri. I följande situationer förblir fjärråtgärden i väntande tillstånd i 30 dagar eller tills enheten bekräftar kommandot när enheten:

- Har ingen anslutning.
- Förlorar sin hanteringsstatus med Intune.

Om du tror att en enhet inte längre checkar in och att den inte tar bort företagsdata väljer du Ta bort. Om du tar bort tas enhetsposten bort så att den inte längre visas i Intune-listan över enheter. För att enheten ska bli aktiv igen måste användaren registrera enheten igen.

F: **Varför är vissa fjärråtgärder inte tillgängliga för mig att använda?**

S: Alla plattformar stöder inte alla fjärrenhetsåtgärder. Följande fjärråtgärder är plattformsspecifika.

- Kringgå aktiveringslås (endast iOS)
- Nystart (endast Windows)
- Förlorat läge (endast iOS)
- Hitta enhet (endast iOS)
- Starta om (endast Windows)

Mer information om varje åtgärd finns i [Tillgängliga enhetsåtgärder](https://docs.microsoft.com/intune/device-management#available-device-actions).