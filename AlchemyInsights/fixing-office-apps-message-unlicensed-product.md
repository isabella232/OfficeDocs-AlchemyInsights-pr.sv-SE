---
title: Det går inte att aktivera Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: de05f869702c40facf61fa5ad01a6ab841b45063
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44499493"
---
# <a name="unable-to-activate-office"></a>Det går inte att aktivera Office

- Kontrollera om prenumerationen har gått ut.
- Kontrollera att du har en prenumeration som tillåter klientlicenser, till exempel Office 365 Business eller Business Premium, och [se till att användaren har en tilldelad licens](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).
- Kontrollera att användaren loggar in i Office med samma konto som tilldelats licensen.
- Gå till sidan för [tjänstens hälsa i Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) för att se om det finns några kända problem med tjänsten.
- Kontrollera brandväggen, antivirusprogram och proxyinställningarna för att kontrollera att de inte blockerar Office-programmens åtkomst till Internet. Gå till [URL-adresser och IP-adressintervall för Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-adresser och IP-adressintervall för Office 365").

- Kontrollera brandväggen, antivirusprogram och proxyinställningarna för att kontrollera att de inte blockerar Office-programmens åtkomst till Internet. Gå till [URL-adresser och IP-adressintervall för Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Använd följande åtgärder för felsökning: 

- Öppna ett Office-program och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton. [Ta bort](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) och [omtilldela](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-licensen och [logga in i Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det påverkade användarkontot.
Använd följande åtgärder för felsökning:

- Öppna ett Office-program och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton. [Ta bort](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users?view=o365-worldwide "Ta bort") och [omtilldela](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide "tilldela om") Office-licensen och [logga in i Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "logga in på Office") med det påverkade användarkontot.
- Kör [Aktiveringsfelsökaren](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Återställ Office-aktiveringsstatus](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Återställa aktiveringstillstånd för Office")
- [Kör en onlinereparation av Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Ytterligare lösningar för felsökning finns i:  
[Office-felmeddelanden om olicensierad produkt och aktivering](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)  
Vi kan inte ansluta till ditt konto. Försök igen senare" fel när du aktiverar Office]( https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 ""Tyvärr, vi kan inte ansluta till ditt konto. Försök igen senare" fel när du aktiverar Office")