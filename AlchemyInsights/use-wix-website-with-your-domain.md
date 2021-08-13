---
title: Använda Wix-webbplats med Office 365 köpta eller hanterade domäner
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
- "9001516"
- "3582"
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980195"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Använda Wix-webbplats med Office 365 köpta eller hanterade domäner

- [Uppdatera DNS-poster för att behålla din webbplats hos ditt nuvarande webbhotell](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix-artikeln "Ansluta en domän till Wix med pekmetoden" rekommenderar att du pekar (lägger till DNS-poster per länken ovan) i stället för att ändra namnservrar när du använder Office 365
- Om du fortfarande väljer att ändra namnservrar till Wix måste du skapa  [DNS-poster på Wix för Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Om domänen har köpts från Microsoft kan namnservrarna inte ändras. Om du måste ändra namnservrar måste den microsoft-köpta domänen överföras  [till en annan värd efter 60 dagar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)