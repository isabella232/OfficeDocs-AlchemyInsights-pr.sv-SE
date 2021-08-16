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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003407"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktivera inbäddning av äldre dialogrutor för att öppna rapporter

**Symptom**

Användare kan inte öppna rapporter. "Något gick fel. Mer information finns i den tekniska informationen."

**Orsak**

Rapporter kan inte läsas in i UCI med felet, "Formulärbeskrivning är null eller inte definierat". Rapporter i UCI kräver fortfarande äldre dialogrutor, så kundens system måste ha *tillåts förlegacydialogsembedding* aktiverat.

**Lösning**

1. Gå till **Inställningar >Administration > System Inställningar > Fliken Allmänt**.

2. Ställ in "Aktivera inbäddning av vissa äldre dialogrutor i Unified Interface-webbläsarklienten" till **Ja.**
