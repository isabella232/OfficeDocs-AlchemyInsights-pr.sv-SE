---
title: 2419-kompatib kan inte möjliggöra revision
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510446"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="9cc26-102">Det går inte att aktivera enhetlig granskning</span><span class="sxs-lookup"><span data-stu-id="9cc26-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="9cc26-103">NÃ¤r du fÃ¶rsÃ¶k fÃ¶rsÃ¶k att aktivera enhetlig granskning fÃ¶r din organisation kan ett felmeddelande visas fÃ¶rsÃ¶k:</span><span class="sxs-lookup"><span data-stu-id="9cc26-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="9cc26-104">Så här löser du problemet:</span><span class="sxs-lookup"><span data-stu-id="9cc26-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="9cc26-105">[Anslut till Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="9cc26-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="9cc26-106">Kör följande cmdlet:</span><span class="sxs-lookup"><span data-stu-id="9cc26-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="9cc26-107">Vänta i 60 minuter innan den föregående inställningen börjar gälla.</span><span class="sxs-lookup"><span data-stu-id="9cc26-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="9cc26-108">Kör följande kommando i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="9cc26-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="9cc26-109">Mer information finns i följande artiklar:</span><span class="sxs-lookup"><span data-stu-id="9cc26-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="9cc26-110">Ansluta till Exchange Online PowerShell med multifaktorautentisering</span><span class="sxs-lookup"><span data-stu-id="9cc26-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="9cc26-111">Aktivera och inaktivera granskningsloggsökning</span><span class="sxs-lookup"><span data-stu-id="9cc26-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
