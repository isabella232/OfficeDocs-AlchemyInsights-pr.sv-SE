---
title: Konfigurera DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808725"
---
# <a name="setup-dkim"></a>Konfigurera DKIM

Fullständiga anvisningar för hur du konfigurerar DKIM för anpassade domäner i Microsoft 365 är [här](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. För **varje** anpassad domän måste du skapa **två** DKIM CNAME-poster hos din domäns DNS-värd (vanligt vis domän registratorn). Contoso.com och fourthcoffee.com kräver exempelvis fyra DKIM CNAME-poster: två för contoso.com och två för fourthcoffee.com.

   DKIM CNAME-poster för **varje** egen domän använder följande format:

   - **Värdnamn**: `selector1._domainkey.<CustomDomain>`

     **Pekar på adress eller värde**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Värdnamn**: `selector2._domainkey.<CustomDomain>`

     **Pekar på adress eller värde**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> är texten till vänster om `.mail.protection.outlook.com` i den anpassade MX-posten för den anpassade domänen (till exempel `contoso-com` för domänen contoso.com). \<InitialDomain\> är den domän du använde när du registrerade dig för Microsoft 365 (till exempel contoso.onmicrosoft.com).

2. När du har skapat CNAME-posterna för dina egna domäner gör du följande:

   a. [Logga in på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med ditt arbets-eller skol konto.

   b. Välj ikonen för startprogrammet i det övre vänstra hörnet, och välj sedan **Admin**.

   c. I den nedre vänstra navigeringen expanderar du **Administratör** och väljer **SharePoint**.

   d. Gå till **skydd**  >  **DKIM**.

   e. Välj domänen och välj **Aktivera** för **signera meddelanden för den här domänen med DKIM-signaturer**. Upprepa det här steget för varje anpassad domän.
