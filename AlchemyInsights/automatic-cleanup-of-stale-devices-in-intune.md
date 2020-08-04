---
title: Automatisk rensning av inaktuella enheter i Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555735"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatisk rensning av inaktuella enheter i Intune

Intune gör det möjligt för administratören att konfigurera ett tidsintervall mellan 90 och 270 dagar, varefter inaktuella enheter tas bort från tjänsten. Den här inställningen är organisationsomfattande och när den aktiveras träder i kraft omedelbart. Alla enheter som inte checkats in på Intune-servern under en period som överskrider inställningen tas bort permanent.

**Anm.)** Endast MDM-enhetsobjekt kan rensas. EAS endast enhetsobjekt är uteslutna.

För ytterligare information om när en enhet blir berättigad till borttagning baserat på enhetens rensning och dess "tillstånd":

Inställning: **Ta bort enheter efter senaste incheckningsdatum: Ja (något värde (N) i angivna dagar)**

- Baserat på värdet (N) som konfigurerats i inställningen tar Intune-tjänsten bort enheten under de angivna dagarna efter att den senast lyckades checka in.

Inställning: **Ta bort enheter efter senaste incheckningsdatum: Nej**

- 180 dagar efter att enhetscertifikatet har gått ut och inte förnyats tas enheten bort.

**Anm.)** I båda fallen måste enheten registreras i Intune. Registrering sker under den första enhetsincheckningen med Intune-tjänsten.

Om en enhet registreras framgångsrikt till Intune men inte blir Intune registrerad, tas enheten bort 270 dagar efter registreringen. (90 dagar för att markera enheten som återkallad och sedan ytterligare 180 dagar för att ta bort posten.)

Det finns för närvarande ingen mekanism i Intune-konsolen för att fastställa utgångsdatumet för enhetscertifieringen för en viss enhet.