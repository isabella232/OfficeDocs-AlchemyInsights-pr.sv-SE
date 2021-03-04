---
title: Synkroniseringsfel för automatisk enhetsregistrering för Apple
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
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448940"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Synkroniseringsfel för automatisk enhetsregistrering för Apple

"Vi har upptäckt att du har en eller flera ADE/DEP-token som är i ett felläge. Tills feltillståndet har lösts för varje påverkad token fungerar inte ADE-funktionerna som förväntat."

Det här felet kan visa sig på flera olika sätt, bland annat:

1. Enheter kan inte synkronisera från ABM/ASM till Intune
2. Profiltilldelningar i registrering kanske inte fungerar
3. Enheter kanske inte slutför ADE-registreringen

Kontrollera om synkroniseringsfelet har rapporterats på Intune-konsolen under Enheter > Registrera enheter **> Apple-registrering > token för registreringsprogram.**

En av de vanligaste orsakerna till synkroniseringsfel är att den aktuella tokenet förfaller. I många fall löser förnyelsen av den aktuella tokenen problemet.

Om en eller flera av dina token har upphört att gälla kan du läsa följande dokumentation som hjälper dig att förnya dem efter behov:

[Förnya en token för automatisk enhetsregistrering](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Dessutom kan du se följande dokumentation för att se möjliga åtgärder för andra fel som orsakar tokensynkroniseringsfel:

[ABM-/ASM-synkroniseringsfel för iOS-/iPadOS- och macOS-token för automatisk enhetsregistrering](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM-/ASM-synkroniseringsfel för iOS-/iPadOS- och macOS-token för automatisk enhetsregistrering](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
