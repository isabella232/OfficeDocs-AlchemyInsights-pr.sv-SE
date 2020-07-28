---
title: Hitta förlorade iOS-enheter med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440430"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Hitta förlorade iOS-enheter med Intune

Om du aktiverar förlorat läge på en iOS-enhet kan en administratör få ett meddelande och ett kontakttelefonnummer att visas på låsskärmen.

När förlorat läge är aktiverat kan administratören använda åtgärden Hitta enhet för att identifiera enhetens fysiska plats.

Åtgärden Hitta enhet i Intune fungerar med iOS-enheter för att visa platsen för en viss enhet på en karta.

Om du använder den här åtgärden måste iOS-enheten vara i:

- Övervakat läge
- Förlorat läge

Mer information finns i [Aktivera förlorat läge på iOS/iPadOS-enheter med Intune](https://docs.microsoft.com/intune/device-lost-mode) och Hitta förlorade eller stulna [iOS/iPadOS-enheter med Intune](https://docs.microsoft.com/intune/device-locate).

**FAQ**

F: Jag utfärdade en fjärråtgärd för att ta bort företagsdata från en enhet, och nu har den fastnat i ett väntande tillstånd.

S: För att en fjärråtgärd ska kunna slutföras måste den riktade enheten vara online och felfri. I följande situationer förblir fjärråtgärden i väntande tillstånd i 30 dagar eller tills enheten bekräftar kommandot:

- När enheten inte har anslutning
- När enheten förlorar sin hanteringsstatus med Intune

Om du tror att en enhet inte längre checkar in och att den inte kan ta bort företagsdata väljer du Ta bort. Om du tar bort tas enhetsposten bort så att den inte längre visas i Intune-listan över enheter. Om enheten blir aktiv igen måste användaren registrera den igen.

F: Varför är vissa fjärråtgärder inte tillgängliga för mig att använda?

S: Alla plattformar stöder inte alla fjärrenhetsåtgärder. Följande fjärråtgärder är plattformsspecifika, så de är endast tillgängliga för de noterade plattformarna.

- Kringgå aktiveringslås (endast iOS)
- Nystart (endast Windows)
- Förlorat läge (endast iOS)
- Hitta enhet (endast iOS)
- Starta om (endast Windows)

Mer information om varje åtgärd finns i [Tillgängliga enhetsåtgärder](https://docs.microsoft.com/intune/device-management#available-device-actions).