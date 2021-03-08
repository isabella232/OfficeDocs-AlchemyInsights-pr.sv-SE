---
title: Konfigurera DKIM med egna domäner
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525421"
---
# <a name="set-up-dkim-with-custom-domains"></a>Konfigurera DKIM med egna domäner

Du måste publicera två CNAME-poster för varje anpassad domän i DNS. Det gör du genom att använda följande format:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** är texten till vänster om **.mail.protection.outlook.com** i den anpassade MX-posten för den anpassade domänen (till exempel contoso-com för domänen **contoso.com**). **InitialDomain** är den domän som du använde när du registrerade dig för Office 365 (till **exempel contoso.onmicrosoft.com).**

Mer information om DNS-poster finns i [Skapa DNS-poster hos valfri DNS-värd för Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)