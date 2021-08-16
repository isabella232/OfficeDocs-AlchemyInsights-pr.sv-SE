---
title: Intune-enhetsinventering
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
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014090"
---
# <a name="intune-device-inventory"></a>Intune-enhetsinventering

Bladet Enheter ger administratörsinsikter på enheter under hantering i Intune per enhet. Informationen som visas omfattar: Maskinvara, Identifierade program, Tillstånd för enhetsefterlevnad och Enhetskonfiguration.

Lagerdata för maskinvara och identifierade program samlas in under en sjudagarscykel. Vilka program och specifika delar av maskinvara som rapporteras varierar beroende på enhetens operativsystem och om enheten personligen eller företaget ägs.

Mer information finns i [Visa enhetsinformation i Intune](https://docs.microsoft.com/intune/device-inventory).

**FAQ**

F: Jag får inte en fullständig lagerlista med program som finns på Intune-registrerade Windows enheter. Varför inte?

S: För stunden finns endast moderna appar listade för Windows 10-datorer som identifieras som företagsenheter. Intune samlar inte in information om Win32-appar som är installerade på dessa enheter.

F: Varför samlas inte telefonnummer in från alla enheter?

S: Telefoner som kategoriserats som företagsenheter i Intune identifieras inte med deras fullständiga telefonnummer när du till exempel kör en inventeringsrapport för mobila enheter. Telefonnummer med egen enhet är alltid delvis maskerade med asterisker (****) och endast de sista fyra siffrorna visas.