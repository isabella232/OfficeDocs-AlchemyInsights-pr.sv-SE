---
title: Problem med att ta bort en offboardad eller inaktiverad enhet från enhetsinventeringen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 6eb59d16a1dab2de0e7a44faf9b34be6432342f9e20c94b6932e69e937751add
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892021"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problem med att ta bort en offboardad eller inaktiverad enhet från enhetsinventeringen

Microsoft Defender för Slutpunkt tillåter för närvarande inte att enhetsposten för en offboarded eller inaktiv enhet tas bort manuellt från enhetsinventeringen.

Av säkerhetsskäl finns enheten kvar i portalen som en historisk post i upp till 180 dagar. Men enhetens data rensas enligt din konfigurerade lagringstid.

**Obs!** En offboarded eller inaktiv enhet växlar automatiskt till **inaktivt** läge efter sju dagar. Dessutom räknas inte enheter som inte är aktiva de senaste 30 dagarna in i de data som återspeglar din organisation Hantering av hot och säkerhetsrisker exponeringsresultat eller Microsoft Secure Score för enheter.
 
Om du fortfarande inte vill se vissa enheter i vyn Enhetsinventering kan du prova att placera en enhetstagg för att filtrera bort den inaktiverade enheten från vyn Enhetsinventering.

Mer information finns i:

[Offboard-enheter från Microsoft Defender för Slutpunkt-tjänsten](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Exponeringsresultat i Hantering av hot och säkerhetsrisker](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Åtgärda defekta sensorer i Microsoft Defender för Endpoint](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Så här använder du taggningen effektivt (del 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Så här använder du taggningen effektivt (del 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Så här använder du taggningen effektivt (del 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




