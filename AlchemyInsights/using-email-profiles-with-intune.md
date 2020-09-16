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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653306"
---
# <a name="using-email-profiles-with-intune"></a>Använda e-postprofiler med Intune

Intune kan användas för att skapa och distribuera e-postprofiler för den inbyggda (inbyggda) e-postklienten på flera plattformar.

Information om några av de begränsningar som gäller för e-profiler, inklusive hur befintliga profiler hanteras och hur du tar bort e-profilerna, finns i avsnittet [lägga till inställningar för e-post på enheter med Intune](https://docs.microsoft.com/intune/email-settings-configure).

Mer information om hur du skapar e-postprofiler för varje enhets plattform finns i:

[Android-enhetens inställningar för att konfigurera e-post, auktorisering och synkronisering i Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Lägga till e-postinställningar för iOS-och iPad-enheter i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Inställningar för e-postprofil i Microsoft Intune för enheter med Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Inställningar för e-postprofil för enheter med Windows 10 i Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Vanligt problem med synkronisering**

**En KNOX on Android-e-postprofil hindrar att användarnas kontakter, kalender och uppgifter synkroniseras till användar enheter.**

I e-postprofilen KNOX på Android KNOX kan administratören välja att avgöra vilka innehålls typer som synkroniseras till enheten genom att ställa in dem på aktive rad.

Om inställningen för någon av innehålls typerna är inställd på **ej konfigurerad** (standard) synkroniseras inte den innehålls typen automatiskt. En användare kan aktivera den innehålls typ de vill ha direkt på enheten, men denna konfiguration skrivs över av Intune-inställningarna och synkroniseringen stoppas för innehålls typen.

