---
title: Synkroniseringsfel för Apple Automatisk enhetsregistrering
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
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013766"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synkroniseringsfel för Apple Automatisk enhetsregistrering

"Vi har upptäckt att du har en eller flera ADE/DEP Tokens som har ett feltillstånd. Tills feltillståndet har lösts för varje påverkad token fungerar ADE-funktionen inte som förväntat.".

Det här felet kan visa sig på flera olika sätt:

1. Enheter kan inte synkroniseras från ABM/ASM till Intune
2. Registreringsprofiltilldelningar kanske inte fungerar
3. Enheter kanske inte slutför ADE-registreringen

Kontrollera om synkroniseringsfelet har rapporterats i Intune-konsolen under Enheter > Registrera enheter **> Apple-registrering > Token** för registreringsprogram .

En av de vanligaste orsakerna till synkroniseringsfel är förfallotiden för den aktuella tokenen. I många fall löses problemet om den aktuella tokenen förnyas.

Om en eller flera av dina token har upphört att gälla kan du läsa följande dokumentation som hjälper dig att förnya dem efter behov:

[Förnya en token för automatisk enhetsregistrering](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Dessutom kan du se följande dokumentation för att se möjliga åtgärder för andra fel som orsakar tokensynkroniseringsfel:

[ABM-/ASM-synkroniseringsfel för iOS-/iPadOS- och macOS-automatiska token för enhetsregistrering](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM-/ASM-synkroniseringsfel för iOS-/iPadOS- och macOS-automatiska token för enhetsregistrering](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
