---
title: Konfigurera DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509402"
---
# <a name="setup-dkim"></a>Konfigurera DKIM

De fullständiga instruktionerna för att konfigurera DKIM för anpassade domäner i Microsoft 365 finns [här](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. För **varje** anpassad domän måste du skapa **två** DKIM CNAME-poster på domänens DNS-värdtjänst (vanligtvis domänregistratorer). Till exempel kräver contoso.com och fourthcoffee.com fyra DKIM CNAME-poster: två för contoso.com och två för fourthcoffee.com.

   DKIM CNAME-posterna för **varje** anpassad domän använder följande format:

   - **Värdnamn:**`selector1._domainkey.<CustomDomain>`

     **Pekar på adress eller värde:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Värdnamn:**`selector2._domainkey.<CustomDomain>`

     **Pekar på adress eller värde:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>är texten till vänster `.mail.protection.outlook.com` om i den anpassade MX-posten för den anpassade domänen (till exempel för `contoso-com` domänen contoso.com). \<InitialDomain\>är den domän som du använde när du registrerade dig för Microsoft 365 (till exempel contoso.onmicrosoft.com).

2. När du har skapat CNAME-posterna för dina anpassade domäner gör du följande instruktioner:

   a. [logga in på Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) med ditt arbets- eller skolkonto.

   b. Välj ikonen för startprogrammet i det övre vänstra hörnet, och välj sedan **Admin**.

   c. I den nedre vänstra navigeringen expanderar du **Administratör** och väljer **SharePoint**.

   d. Gå till **Skydd**  >  **DKIM**.

   e. Välj domänen och välj sedan **Aktivera** för **signeringsmeddelanden för den här domänen med DKIM-signaturer**. Upprepa det här steget för varje anpassad domän.
