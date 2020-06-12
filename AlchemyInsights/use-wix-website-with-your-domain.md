---
title: Använda Wix-webbplats med köpta eller hanterade Office 365-domäner
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
ms.openlocfilehash: 64dfe6082bea1e468eae78bf1576fde398e4c28a
ms.sourcegitcommit: 3ca312535d950105ee829e037f0ff8f1ddbbae72
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/11/2020
ms.locfileid: "44708502"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Använda Wix-webbplats med köpta eller hanterade Office 365-domäner

- [Uppdatera DNS-poster för att hålla din webbplats med din nuvarande värdleverantör](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix-artikeln "Ansluta en domän till Wix Med hjälp av pekningsmetoden" rekommenderar du att du använder pekning (lägga till DNS-poster per länken ovan) i stället för att byta namnservrar när du använder Office 365
- Om du fortfarande väljer att ändra namnservrar till Wix måste du skapa [DNS-poster på Wix för Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Om din domän köptes från Microsoft kan inte namnservrarna ändras. Om du måste ändra namnservrar måste Den köpta Microsoft-domänen [överföras till en annan värdleverantör efter 60 dagar](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)