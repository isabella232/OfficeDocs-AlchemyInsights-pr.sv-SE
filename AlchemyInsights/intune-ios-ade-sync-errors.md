---
title: Automatiska synkroniseringsfel för automatisk enhets registrering
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714974"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Automatiska synkroniseringsfel för automatisk enhets registrering

"Vi har upptäckt att du har en eller flera ADE-token i ett fel tillstånd. Tills felet är löst för varje token fungerar inte ADE-funktionen för samma ".

Det här felet kan uppstå på flera olika sätt:

1. Enheter kan inte synkroniseras från ABM/ASM till Intune
2. Profil tilldelningar kan Miss lyckas
3. Enheter kan inte slutföra en ofullständig ADE-registrering

Kontrol lera det synkroniseringsfel som rapporter ATS i Intune-konsolen under **enheter > registrera enheter > > Apples registrerings program** och granska följande dokumentation för att se eventuell reparation:

[ABM/ASM sync-fel för iOS/iPad och macOS automatisk enhets registrerings-token](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
