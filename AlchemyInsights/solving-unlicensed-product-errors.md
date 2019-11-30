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
ms.openlocfilehash: 178811c81775b22676a0106283be4e516d40a95b
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628044"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Förslag för att lösa "olicensierad produkt" fel

Försök med följande för att lösa fel om en "olicensierad produkt":

- Kontrollera om din prenumerationsstatus har upphört att gälla.
- Kontrollera att du har en prenumeration som tillåter klientlicenser, till exempel Office 365 Business eller Business Premium, och [Se till att användaren har en tilldelad licens](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users). 
- Kontrollera att användaren loggar in på Office med samma konto som har tilldelats licensen.
- Kontrollera [Office 365 service Health-sidan](https://docs.microsoft.com/office365/enterprise/view-service-health) för att se om det finns några kända problem med tjänsten.
- Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Office-apparna tillgång till Internet. Se [Office 365-URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Du kan också prova följande felsökningsåtgärder: 

- Öppna en Office-app och [Logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från alla befintliga användarkonton. [Ta bort](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users) och tilldela Office-licensen [igen](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) och logga sedan in på [Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det aktuella användarkontot.
- Kör [felsökaren för aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Återställ aktiveringstillståndet för Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Utför en onlinereparation av Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Ytterligare felsökningslösningar finns i: 

- [Olicensierad produkt och aktiveringsfel i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- ["Vi kan tyvärr inte ansluta till ditt konto. Försök igen senare "felmeddelande när du aktiverar Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)