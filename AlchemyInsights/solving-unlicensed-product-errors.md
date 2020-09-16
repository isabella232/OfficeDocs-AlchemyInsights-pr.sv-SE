---
title: Lösa problem med olicensierad produkt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737971"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Förslag på problem med "olicensierad produkt"

Gör så här för att lösa problem med en "olicensierad produkt":

- Kontrol lera om din prenumerations status har gått ut.
- Kontrol lera att du har en prenumeration som tillåter klient licenser, till exempel Microsoft 365-appar för företag eller Business Premium, och [Se till att användaren har en tilldelad licens](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Kontrol lera att användaren loggar in på Office med samma konto som har tilldelats licensen.
- Kontrol lera [tjänstens hälso sida](https://docs.microsoft.com/office365/enterprise/view-service-health) för att se om det finns kända problem med tjänsten.
- Kontrol lera brand vägg, antivirus program och proxyinställningar för att bekräfta att de inte blockerar Microsoft 365-appar till Internet. Se [URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Du kan också försöka med följande fel söknings åtgärder: 

- Öppna ett Office-program och [Logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användar konton. [Ta bort](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) och [tilldela om](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-licensen och logga sedan [in på Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det användar konto som påverkas.
- Kör [fel sökaren för aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Återställ Office-aktiveringsstatusen](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Utföra en online-reparation av Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Ytterligare lösningar för felsökning finns i: 

- [Office-felmeddelanden om olicensierad produkt och aktivering](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Felet "Det går inte att ansluta till ditt konto. Försök igen senare" visas när du aktiverar Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)