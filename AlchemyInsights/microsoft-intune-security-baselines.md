---
title: Använda Microsoft Intune säkerhetsbaslinjer för att konfigurera Windows 10 enheter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 911c6b1860e4f44e6d88897f73173cdd11060562
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332003"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Använda Microsoft Intune säkerhetsbaslinjer för att konfigurera Windows 10 enheter

Intune-säkerhetsbaslinjer hjälper till att skydda användare och enheter. Säkerhetsbaslinjer är Windows förkonfigurerade grupper som används för att tillämpa en känd grupp med inställningar och standardvärden som rekommenderas av relevanta säkerhetsteam. Genom att skapa en profil för säkerhetsbaslinje i Intune skapar du en mall som består av flera enhetskonfigurationsprofiler.

När du distribuerar säkerhetsbaslinjer till grupper av användare eller enheter tillämpas inställningarna på enheter som körs Windows 10 eller senare. Microsofts baslinje för hantering av mobila enheter (MDM) aktiverar till exempel automatiskt BitLocker för flyttbara enheter, kräver lösenordet för att låsa upp en enhet och inaktiverar grundläggande autentisering. När ett standardvärde inte fungerar för din miljö kan du anpassa originalplanen så att de inställningar du behöver används.

Säkerhetsbaslinjer hjälper också till att upprätta ett säkert arbetsflöde av helt slut i Microsoft 365. En säkerhetsbaslinje innehåller metodtips och rekommendationer för inställningar som påverkar säkerheten. Intune-partner med Windows säkerhetsteam som skapar baslinjer för gruppprinciper, så dessa rekommendationer baseras på stabil vägledning och omfattande erfarenhet.

Om du är nybörjare i Intune och är osäker på var du ska börja kan du med hjälp av säkerhetsbaslinjer snabbt skapa och distribuera en säker profil. Om du använder en grupprincip är det mycket enklare att migrera till Intune för hanteringsändamål med säkerhetsbaslinjer eftersom de är inbyggda i Intune och innehåller avancerade hanteringsfunktioner.

Mer information finns i Windows [baslinjer för säkerhet](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) och [hantering av mobila enheter.](https://docs.microsoft.com/windows/client-management/mdm/)

