---
title: Utfasning av Exchange PowerShell och grundläggande autentisering
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813490"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Utfasning av Exchange PowerShell och grundläggande autentisering

Om du vill ha den senaste informationen om hur du ansluter till Exchange Online PowerShell utan att använda grundläggande autentisering [går du hit](https://aka.ms/exops-docs). PowerShell V2-modulen använder inte grundläggande autentisering.

Observera att grundläggande autentisering fortfarande måste aktiveras på klientdatorn.
Den nya PowerShell V2-modulen använder modern autentisering för att upprätta anslutning och möjliggöra alla REST-baserade V2-cmdletar. Utöver V2-cmdletar kan du också komma åt äldre PowerShell-cmdletar (RPS) som kräver en PowerShell-fjärrsession för att upprättas. Att upprätta en RPS-session på en Windows-dator kräver grundläggande WinRM-autentisering för att kunna aktiveras på klientdatorn även om modulen använder en mekanism med modern autentisering för att autentisera för tjänsten. Pipeline för grundläggande WinRM-autentisering används för att transportera token för modern autentisering. Om grundläggande WinRM-autentisering är inaktiverat på klientdatorn fortsätter de nya V2-cmdletar att fungera (men inte de äldre RPS-cmdletarna).
