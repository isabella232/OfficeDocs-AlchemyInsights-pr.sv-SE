---
title: Enhets inventering i Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667896"
---
# <a name="intune-device-inventory"></a>Enhets inventering i Intune

Med enheten enheter får administratören en inblick i enheter under hantering i Intune per enhet. Informationen som visas är: maskin vara, upptäckta program, enhetens kompatibilitetsstatus och status för enhets konfiguration.

Lager data för hård vara och upptäckta program samlas in på sju dagar. Vilka program och specifika delar av maskin varan som rapporteras varierar beroende på enhetens operativ system och om enheten är personligen eller ägda.

Mer information finns i [Se enhets detaljer i Intune](https://docs.microsoft.com/intune/device-inventory).

**FAQ**

F: Jag får inte en fullständig inventering av program som finns på Intune-registrerade Windows-enheter. Varför inte?

A: i det här fallet visas bara moderna appar för Windows 10-datorer som identifieras som företags enheter. Intune samlar inte in information om Win32-program som är installerade på dessa enheter.

F: Varför hämtas inte telefonnummer från alla enheter?

A: telefoner kategoriserade som företags enheter i Intune identifieras inte med deras fullständiga telefonnummer när du till exempel kör en inventerings rapport för mobila enheter. Fasta enheter telefonnummer är alltid delvis maskerade med asterisker (* * * *) och bara visa de fyra sista siffrorna.