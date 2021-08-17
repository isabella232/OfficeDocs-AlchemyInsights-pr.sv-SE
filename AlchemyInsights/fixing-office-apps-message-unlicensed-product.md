---
title: Det gick inte att aktivera Office
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
- "2000023"
- "3509"
ms.openlocfilehash: eb62dfce9f9507dd8806d91343cd39fe76e65594473683c1393d524f6c2d8a27
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893929"
---
# <a name="unable-to-activate-office"></a>Det gick inte att aktivera Office

**Obs!** Om du använder en äldre version av Windows (till exempel Windows 7) ska du kontrollera att TLS 1.2 är aktiverat som standard. Mer information finns i Uppdatering för att aktivera [TLS 1.1 och TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard säkra protokoll i WinHTTP i Windows.

- Kontrollera om prenumerationen har gått ut.
- Kontrollera att du har en prenumeration som tillåter klientlicenser som exempelvis Office 365 Business eller Business Premium, samt att [användaren har en licens tilldelad](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Kontrollera att användaren loggar in i Office med samma konto som tilldelats licensen.
- Gå till [sidan för tjänststatus i Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) för att se om det finns några kända problem med tjänsten.
- Kontrollera brandväggen, antivirusprogram och proxyinställningarna för att kontrollera att de inte blockerar Microsoft 365-applikationers åtkomst till internet. Gå till [URL-adresser och IP-adressintervall för Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-adresser och IP-adressintervall för Office 365").

**Tips** På Windows-datorer kan vi diagnostisera och automatiskt korrigera flera vanliga inloggningsproblem för Office åt dig. Ladda ned och kör **[Support- och återställningsassistenten](https://aka.ms/SaRA-OfficeSignInScenario)** om du vill använda vårt automatiska verktyg.

Använd följande åtgärder för felsökning:

- Öppna ett Office-program och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton. [Ta bort](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) och [omtilldela](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-licensen och [logga in i Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det påverkade användarkontot.
- Kör [Aktiveringsfelsökaren](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Återställ Office-aktiveringsstatus](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Återställ Office-aktiveringsstatus")
- [Kör en onlinereparation av Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Ytterligare lösningar för felsökning finns i:  

- [Office-felmeddelanden om olicensierad produkt och aktivering](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Felet "Det går inte att ansluta till ditt konto. Försök igen senare" visas när du aktiverar Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)