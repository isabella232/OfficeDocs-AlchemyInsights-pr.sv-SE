---
title: Använda säkerhets bas linjer i Microsoft Intune för att konfigurera Windows 10-enheter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573787"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Använda säkerhets bas linjer i Microsoft Intune för att konfigurera Windows 10-enheter

Intune säkerhets bas linjer hjälper dig att skydda användare och enheter. Säkerhets bas linjer är Windows-inställningar ' förkonfigurerade grupper som används för att tillämpa en känd uppsättning inställningar och standardvärden som rekommenderas av relevanta säkerhets team. Genom att skapa en säkerhets bas profil i Intune skapar du en mall som består av flera enheter-konfigurations profiler.

När du distribuerar säkerhets bas linjer till grupper med användare eller enheter tillämpas inställningarna på enheter som körs på Windows 10 eller senare. Till exempel kan MDM-säkerhetsfunktionen (1) Aktivera BitLocker för flyttbara enheter (2) kräva lösen ordet för att låsa upp en enhet och (3) inaktiverar grundläggande verifikation. När ett standardvärde inte fungerar för din miljö kan du anpassa bas linjen för att tillämpa de inställningar du behöver.

Säkerhets bas linjer hjälper dig också att etablera ett säkert arbets flöde från ett slutdatum till en slutpunkt i Microsoft 365. Här är några av fördelarna med följande:

- En säkerhets plan innehåller de bästa metoderna och rekommendationerna för inställningar som påverkar säkerheten. Eftersom Intune-partners med Windows säkerhets team som skapar bas linjer för grup principer baseras dessa rekommendationer på heltäckande vägledning och omfattande upplevelse.
- Om du är nybörjare på Intune och är osäker på var du ska starta, kan du med hjälp av säkerhets rikt linjer snabbt skapa och distribuera en säker profil.
- Om du för närvarande använder en grup princip är det mycket enklare att migrera till Intune för hantering med säkerhets bas linjer, eftersom de är inbyggda i Intune och innehåller funktioner för överkanten för hantering.

Mer information finns i [säkerhets bas linjer för Windows](https://go.microsoft.com/fwlink/?linkid=2141503) och [hantering av mobila enheter](https://go.microsoft.com/fwlink/?linkid=2141701).