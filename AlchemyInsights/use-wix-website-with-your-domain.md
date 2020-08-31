---
title: Använda WIX webbplats med Office 365-köpta eller hanterade domäner
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300742"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Använda WIX webbplats med Office 365-köpta eller hanterade domäner

- [Uppdatera DNS-poster för att behålla din webbplats med din nuvarande värd](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- WIX artikeln "ansluta en domän till WIX med metoden Point" rekommenderar att du använder pekdon (lägga till DNS-poster per länken ovan) i stället för att byta namn på servrar när du använder Office 365
- Om du fortfarande väljer att ändra namnservrar till WIX måste du  [Skapa DNS-poster på WIX för Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Om din domän har köpts från Microsoft kan namnservrar inte ändras. Om du behöver ändra namn servrar måste Microsoft-domänen vara  [överföra till en annan värd efter 60 dagar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)