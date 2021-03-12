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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747635"
---
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="79a78-102">Konfigurera DKIM med anpassade domäner</span><span class="sxs-lookup"><span data-stu-id="79a78-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="79a78-103">Du måste publicera två CNAME-poster för varje anpassad domän i DNS.</span><span class="sxs-lookup"><span data-stu-id="79a78-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="79a78-104">Det gör du genom att använda följande format:</span><span class="sxs-lookup"><span data-stu-id="79a78-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="79a78-105">**DomainGUID** är texten till vänster om **.mail.protection.outlook.com** i den anpassade MX-posten för den anpassade domänen (till exempel contoso-com för **contoso.com**).</span><span class="sxs-lookup"><span data-stu-id="79a78-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="79a78-106">**InitialDomain** är den domän som du använde när du registrerade dig för Office 365 (till exempel **contoso.onmicrosoft.com**).</span><span class="sxs-lookup"><span data-stu-id="79a78-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="79a78-107">Mer information om DNS-poster finns i [Skapa DNS-poster på vilken DNS-värd som helst för Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="79a78-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>