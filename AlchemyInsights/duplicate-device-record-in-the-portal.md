---
title: Dubblerad enhetspost i portalen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790175"
---
# <a name="duplicate-device-record-in-the-portal"></a>Dubblerad enhetspost i portalen

Du kan se två poster för en enhet i portalen om enheten inte korrekt rapporterar status för samhantering till Configuration Manager-webbplatsen. För att kontrollera statusen för samhantering av en enhet tittar du i kolumnen **Samhanterad** för enheten i Configuration Manager-konsolen. Om kolumnen inte visas kan du lägga till den genom att högerklicka på en kolumnrubrik och välja den i listan.

Värdet på Samhanterad ska vara **Ja**. Om värdet är **Nej** öppnar du Configuration Manager-klientappleten på klientenheten och markerar egenskapen **Samhantering** på fliken Allmänt.

- Om värdet är **Aktiverat** antyder det problem med klientkommunikationen med hanteringsplatsen. Läs **CcmMessaging.log** på enheten för att undersöka potentiella anslutningsproblem.

- Om värdet är **Inaktiverat** och enheten är registrerad i Intune ska du kontrollera att enheten har tagit emot principen för samhantering genom att läsa **CoManagementHandler.log** på enheten.
