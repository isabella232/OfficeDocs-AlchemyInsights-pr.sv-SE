---
title: Lösa felmeddelanden om olicensierad produkt
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786867"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Förslag på hur du löser "Olicensierad produkt"-fel

Prova följande för att lösa fel om en "Olicensierad produkt":

- Kontrollera om din prenumerationsstatus har upphört att gälla.
- Kontrollera att du har en prenumeration som tillåter klientlicenser, till exempel Microsoft 365-appar för företag eller Business Premium, och kontrollera att användaren har [en tilldelad licens.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Kontrollera att användaren loggar in på Office med samma konto som licensen har tilldelats.
- Kontrollera sidan [Tjänstens hälsa](https://docs.microsoft.com/office365/enterprise/view-service-health) för att se om det finns kända problem med tjänsten.
- Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att kontrollera att de inte blockerar Microsoft 365-apparna åtkomst till Internet. Se [URL:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Du kan också prova följande felsökningsåtgärder: 

- Öppna ett Office-program [och logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton. [Ta](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) bort [och tilldela Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) igen och logga [sedan in på Office med](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) det aktuella användarkontot.
- Kör [felsökaren för aktivering.](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Återställ Office-aktiveringsstatusen](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Utföra en onlinereparation av Office.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)

Ytterligare lösningar för felsökning finns i: 

- [Office-felmeddelanden om olicensierad produkt och aktivering](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Felet "Det går inte att ansluta till ditt konto. Försök igen senare" visas när du aktiverar Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)