---
title: Setup DKIM i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765473"
---
# <a name="setup-dkim-in-office-365"></a>Setup DKIM i Office 365

Fullständiga instruktioner för hur du konfigurerar DKIM för anpassade domäner i Office 365 är [här](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. För **varje** egen domän måste du skapa **två** DKIM CNAME-poster i din domän DNS-värdtjänsten (vanligtvis domänregistrerare). Till exempel contoso.com och fourthcoffee.com kräver fyra DKIM CNAME-poster: två för contoso.com och två för fourthcoffee.com.

   DKIM CNAME-poster för **varje** anpassad domän använder du följande format:

   - **Värdnamn**:`selector1._domainkey.<CustomDomain>`

     **Punkter till adressen eller värde**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Värdnamn**:`selector2._domainkey.<CustomDomain>`

     **Punkter till adressen eller värde**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> står till vänster om `.mail.protection.outlook.com` i anpassade MX-posten för den egna domänen (till exempel `contoso-com` för domänen contoso.com). \<InitialDomain\> är den domän som du använde när du registrerade dig för Office 365 (till exempel contoso.onmicrosoft.com).

2. När du har skapat CNAME-poster för egna domäner, slutför du följande anvisningar:

   en. [Logga in på Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med ditt arbets- eller skolkonto.

   b. Välj ikonen för startprogrammet i det övre vänstra hörnet och välj **Admin**.

   c. Expandera **Admin** och välj **Exchange**i den nedre vänstra navigeringen.

   d. Gå till **skydd** > **DKIM**.

   e. Välj domän och välj **Aktivera** för att **signera meddelanden för den här domänen med DKIM-signaturer**. Upprepa detta steg för varje egen domän.
