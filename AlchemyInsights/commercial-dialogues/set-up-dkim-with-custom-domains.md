---
title: Konfigurera DKIM med anpassade domäner
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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332325"
---
# <a name="set-up-dkim-with-custom-domains"></a>Konfigurera DKIM med anpassade domäner

Du måste publicera två CNAME-poster för varje anpassad domän i DNS. Det gör du genom att använda följande format:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Obs!** **DomainGUID** är texten till vänster om **.mail.protection.outlook.com** i den anpassade MX-posten för den anpassade domänen (till exempel contoso-com för **contoso.com**). **InitialDomain** är den domän du använde när du registrerade dig för Office 365 (till exempel **contoso.onmicrosoft.com**).

Mer information om DNS-poster finns i [Skapa DNS-poster på vilken DNS-värd som helst för Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)