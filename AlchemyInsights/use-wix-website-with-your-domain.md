---
title: Använda Wix-webbplatsen med köpta eller hanterade domäner i Office 365
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
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825965"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Använda Wix-webbplatsen med köpta eller hanterade domäner i Office 365

- [Uppdatera DNS-poster för att behålla din webbplats hos ditt nuvarande webbhotell](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix-artikeln "Ansluta en domän till Wix med pekmetoden" rekommenderar att du pekar (lägger till DNS-poster per länken ovan) i stället för att ändra namnservrar när du använder Office 365
- Om du fortfarande väljer att ändra namnservrar till Wix måste du skapa  [DNS-poster på Wix för Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Om domänen har köpts från Microsoft kan namnservrarna inte ändras. Om du måste ändra namnservrar måste den microsoft-köpta domänen överföras  [till en annan värd efter 60 dagar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)