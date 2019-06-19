---
title: 2419--till-aktivera-granskning
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065713"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="5beb6-102">Det går inte att aktivera enhetlig granskning</span><span class="sxs-lookup"><span data-stu-id="5beb6-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="5beb6-103">När du försöker aktivera enhetlig granskning för organisationen Office 365 kan du få ett felmeddelande liknande följande:</span><span class="sxs-lookup"><span data-stu-id="5beb6-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="5beb6-104">Lös problemet så här:</span><span class="sxs-lookup"><span data-stu-id="5beb6-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="5beb6-105">[Ansluta till Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="5beb6-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="5beb6-106">Kör du följande cmdlet:</span><span class="sxs-lookup"><span data-stu-id="5beb6-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="5beb6-107">Vänta i 60 minuter för den tidigare inställningen ska börja gälla.</span><span class="sxs-lookup"><span data-stu-id="5beb6-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="5beb6-108">Kör följande kommando i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="5beb6-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="5beb6-109">Mer information finns i följande artiklar:</span><span class="sxs-lookup"><span data-stu-id="5beb6-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="5beb6-110">Ansluta till Exchange Online PowerShell använder autentisering i flera steg</span><span class="sxs-lookup"><span data-stu-id="5beb6-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="5beb6-111">Aktivera och inaktivera Office 365 Granska loggen Sök</span><span class="sxs-lookup"><span data-stu-id="5beb6-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
