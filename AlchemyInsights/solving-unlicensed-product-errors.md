---
title: Lösa olicensierade produktfel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: b629f24014a789b1f9847f62e725f726d4199027
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44512030"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Förslag för att lösa fel i "Olicensierad produkt"

Försök med följande om du vill lösa fel i en olicensierad produkt:

- Kontrollera om din prenumerationsstatus har upphört att gälla.
- Kontrollera att du har en prenumeration som tillåter klientlicenser, till exempel Microsoft 365 Apps for business eller Business Premium, och [se till att användaren har tilldelat en licens](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Kontrollera att användaren loggar in på Office med samma konto som har tilldelats licensen.
- Kontrollera [hälsosidan för tjänsten](https://docs.microsoft.com/office365/enterprise/view-service-health) för att se om det finns några kända problem med tjänsten.
- Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Office-appars åtkomst till Internet. Se [webbadresser och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Du kan också prova följande felsökningsåtgärder: 

- Öppna ett Office-program och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton. [Ta bort](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) och [tilldela Office-licensen igen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) och logga sedan in på [Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det berörda användarkontot.
- Kör [felsökaren för aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Återställ Office-aktiveringsstatusen](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Utför en onlinereparation av Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Ytterligare lösningar för felsökning finns i: 

- [Office-felmeddelanden om olicensierad produkt och aktivering](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Felet "Det går inte att ansluta till ditt konto. Försök igen senare" visas när du aktiverar Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)