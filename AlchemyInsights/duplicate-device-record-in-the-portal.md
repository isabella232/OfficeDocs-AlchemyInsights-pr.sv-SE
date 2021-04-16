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
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814534"
---
# <a name="duplicate-device-record-in-the-portal"></a>Dubblerad enhetspost i portalen

Du kan se två poster för en enhet i portalen om enheten inte korrekt rapporterar status för samhantering till Configuration Manager-webbplatsen. För att kontrollera statusen för samhantering av en enhet tittar du i kolumnen **Samhanterad** för enheten i Configuration Manager-konsolen. Om kolumnen inte visas kan du lägga till den genom att högerklicka på en kolumnrubrik och välja den i listan.

Värdet på Samhanterad ska vara **Ja**. Om värdet är **Nej** öppnar du Configuration Manager-klientappleten på klientenheten och markerar egenskapen **Samhantering** på fliken Allmänt.

- Om värdet är **Aktiverat** antyder det problem med klientkommunikationen med hanteringsplatsen. Läs **CcmMessaging.log** på enheten för att undersöka potentiella anslutningsproblem.

- Om värdet är **Inaktiverat** och enheten är registrerad i Intune ska du kontrollera att enheten har tagit emot principen för samhantering genom att läsa **CoManagementHandler.log** på enheten.
