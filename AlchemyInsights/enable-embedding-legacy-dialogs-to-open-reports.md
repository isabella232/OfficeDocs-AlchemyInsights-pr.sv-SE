---
title: Aktivera inbäddning av äldre dialogrutor för att öppna rapporter
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814282"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktivera inbäddning av äldre dialogrutor för att öppna rapporter

**Symptom**

Användare kan inte öppna rapporter. "Något gick fel. Mer information finns i den tekniska informationen."

**Orsak**

Rapporter kan inte läsas in i UCI med felet, "Formulärbeskrivning är null eller inte definierat". Rapporter i UCI kräver fortfarande äldre dialogrutor, så kundens system måste ha *tillåts förlegacydialogsembedding* aktiverat.

**Lösning**

1. Gå till **Inställningar >Administration > Systeminställningar > Fliken Allmänt.**

2. Ställ in "Aktivera inbäddning av vissa äldre dialogrutor i Unified Interface-webbläsarklienten" till **Ja.**
