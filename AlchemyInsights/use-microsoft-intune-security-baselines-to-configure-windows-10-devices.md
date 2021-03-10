---
title: Använda säkerhetsbaslinjer för Microsoft Intune för att konfigurera Windows 10-enheter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696383"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Använd säkerhetsbaslinjerna för Microsoft Intune för att konfigurera Windows 10-enheter

Intune-säkerhetsbaslinjer hjälper till att skydda användare och enheter. Säkerhetsbaslinjer är Windows-inställningarnas förkonfigurerade grupper som används för att använda en känd grupp med inställningar och standardvärden som rekommenderas av relevanta säkerhetsteam. Genom att skapa en säkerhetsbaslinjeprofil i Intune skapar du en mall som består av flera konfigurationsprofiler för enheter.

När du distribuerar säkerhetsbaslinjer till grupper av användare eller enheter tillämpas inställningarna på enheter som körs på Windows 10 eller senare versioner. Till exempel aktiverar Microsofts baslinje för hantering av mobila enheter (MDM) automatiskt (1) BitLocker för flyttbara enheter, (2) kräver lösenordet för att låsa upp en enhet och (3) inaktiverar grundläggande autentisering. När ett standardvärde inte fungerar för din miljö kan du anpassa baslinjen så att de inställningar du behöver används.

Säkerhetsbaslinjer hjälper också till att upprätta ett säkert arbetsflöde i Microsoft 365. Följande är några av fördelarna med den här funktionen:
- En säkerhetsbaslinje innehåller metodtips och rekommendationer för inställningar som påverkar säkerheten. Eftersom Intune samarbetar med Windows-säkerhetsteamet som skapar baslinjer för grupprinciper, baseras de här rekommendationerna på stabil vägledning och omfattande erfarenhet.
- Om du är nybörjare i Intune och är osäker på var du ska börja kommer säkerhetsbaslinjer att hjälpa dig att snabbt skapa och distribuera en säker profil.
- Om du använder en grupprincip är det mycket enklare att migrera till Intune för hanteringsändamål med säkerhetsbaslinjer, eftersom dessa säkerhetsbaslinjer är inbyggda i Intune och innehåller avancerade funktioner för hantering.

Mer information finns i Windows [säkerhetsbaslinjer och](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) hantering [av mobila enheter.](https://docs.microsoft.com/windows/client-management/mdm/)