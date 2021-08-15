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
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994847"
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
> [!NOTE]
> **DomainGUID** är texten till vänster om **.mail.protection.outlook.com** i den anpassade MX-posten för den anpassade domänen (till exempel contoso-com för **contoso.com**). **InitialDomain** är den domän som du använde när du registrerade dig för Office 365 (till exempel **contoso.onmicrosoft.com**).

Mer information om DNS-poster finns i [Skapa DNS-poster på vilken DNS-värd som helst för Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)