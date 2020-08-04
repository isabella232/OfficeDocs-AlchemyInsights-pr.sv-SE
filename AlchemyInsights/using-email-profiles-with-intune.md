---
title: Använda e-postprofiler med Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555760"
---
# <a name="using-email-profiles-with-intune"></a>Använda e-postprofiler med Intune

Intune kan användas för att skapa och distribuera e-postprofiler för den inbyggda (inbyggda) e-postklienten på flera enhetsplattformar.

Information om några av de begränsningar som är kopplade till e-postprofiler, inklusive hur förekomsten av befintliga profiler hanteras och hur du tar bort e-postprofiler, finns [i Lägga till e-postinställningar på enheter som använder Intune](https://docs.microsoft.com/intune/email-settings-configure).

Mer information om hur du skapar e-postprofiler för varje enhetsplattform finns i:

[Inställningar för Android-enheter för att konfigurera e-post, autentisering och synkronisering i Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Lägga till e-postinställningar för iOS- och iPadOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Inställningar för e-postprofiler i Microsoft Intune för enheter som kör Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Inställningar för e-postprofiler för enheter som kör Windows 10 i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Vanligt synkroniseringsproblem**

**En KNOX på Android-e-postprofil förhindrar att användarna kontakter, kalender och uppgifter synkroniseras med användarenheter.**

Knox på Android KNOX-e-postprofilen ger administratören möjlighet att bestämma vilka innehållstyper som ska synkroniseras med enheten genom att ställa in var och en på aktiverad.

Om inställningen för någon av innehållstyperna är inställd **på Inte konfigurerad** (standard) synkroniseras inte innehållstypen automatiskt. En användare kan aktivera den innehållstyp de vill ha direkt på enheten manuellt, men den konfigurationen skrivs över av principinställningen Intune och synkroniseringen stoppas för den innehållstypen.

