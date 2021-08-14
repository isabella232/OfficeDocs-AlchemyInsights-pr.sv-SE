---
title: Dubblerad enhetspost i portalen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004172"
---
# <a name="duplicate-device-record-in-the-portal"></a>Dubblerad enhetspost i portalen

Du kan se två poster för en enhet i portalen om enheten inte korrekt rapporterar status för samhantering till Configuration Manager-webbplatsen. För att kontrollera statusen för samhantering av en enhet tittar du i kolumnen **Samhanterad** för enheten i Configuration Manager-konsolen. Om kolumnen inte visas kan du lägga till den genom att högerklicka på en kolumnrubrik och välja den i listan.

Värdet på Samhanterad ska vara **Ja**. Om värdet är **Nej** öppnar du Configuration Manager-klientappleten på klientenheten och markerar egenskapen **Samhantering** på fliken Allmänt.

- Om värdet är **Aktiverat** antyder det problem med klientkommunikationen med hanteringsplatsen. Läs **CcmMessaging.log** på enheten för att undersöka potentiella anslutningsproblem.

- Om värdet är **Inaktiverat** och enheten är registrerad i Intune ska du kontrollera att enheten har tagit emot principen för samhantering genom att läsa **CoManagementHandler.log** på enheten.
