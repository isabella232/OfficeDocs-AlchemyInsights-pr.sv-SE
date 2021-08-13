---
title: Använda e-postprofiler med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919441"
---
# <a name="using-email-profiles-with-intune"></a>Använda e-postprofiler med Intune

Intune kan användas för att skapa och distribuera e-postprofiler för den inbyggda e-postklienten på flera enhetsplattformar.

Mer information om några av begränsningarna som är kopplade till e-postprofiler, bland annat hur befintliga profiler hanteras och hur du tar bort e-postprofiler, finns i Lägga till e-postinställningar på enheter med [Intune.](https://docs.microsoft.com/intune/email-settings-configure)

Mer information om hur du skapar e-postprofiler för varje enhetsplattform finns i:

[Android-enhetsinställningar för att konfigurera e-post, autentisering och synkronisering i Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Lägga till e-postinställningar för iOS- och iPadOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Inställningar för e-postprofil Microsoft Intune för enheter med Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Inställningar för e-postprofil för enheter med Windows 10 i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Vanliga synkroniseringsproblem**

**En KNOX på Android-e-postprofil förhindrar att användares kontakter, kalender och uppgifter synkroniseras till användarnas enheter.**

Knox på Android KNOX-e-postprofilen ger administratören möjlighet att avgöra vilka innehållstyper som ska synkroniseras till enheten genom att ange dem som aktiverade.

Om inställningen för någon av innehållstyperna är Ej **konfigurerad** (standard) synkroniseras inte den innehållstypen automatiskt. En användare kan aktivera den innehållstyp som han eller hon vill använda manuellt på enheten, men den konfigurationen skrivs över av Intune-principinställningen och synkroniseringen avbryts för den innehållstypen.

