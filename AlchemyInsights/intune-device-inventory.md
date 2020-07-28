---
title: Intune-enhetslager
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440478"
---
# <a name="intune-device-inventory"></a>Intune-enhetslager

Bladet Enheter ger administratören insikt i enheter under hantering i Intune per enhet. Informationen som visas innehåller: Maskinvara, identifierade program, enhetsefterlevnadstillstånd och enhetskonfiguration.

Inventeringsdata för maskinvara och identifierade program samlas in på en sjudagarscykel. Programmen och specifika delar av maskinvara som rapporteras skiljer sig åt beroende på enhetens operativsystem och om enheten ägs personligen eller i företaget.

Mer information finns [i Se enhetsinformation i Intune](https://docs.microsoft.com/intune/device-inventory).

**FAQ**

F: Jag får inte en fullständig inventeringslista över program som finns på Intune-registrerade Windows-enheter. Varför inte?

S: För närvarande visas endast moderna appar för Windows 10-datorer som identifieras som företagsenheter. Intune samlar inte in information om Win32-appar som är installerade på dessa enheter.

F: Varför samlas inte telefonnummer in från alla enheter?

S: Telefoner som kategoriseras som företagsenheter i Intune identifieras inte med sitt fullständiga telefonnummer när du till exempel kör en inventeringsrapport för mobila enheter. Telefonnummer för bring-you-own-enhet är alltid delvis maskerade med asterisker (****) och visar bara de fyra sista siffrorna.