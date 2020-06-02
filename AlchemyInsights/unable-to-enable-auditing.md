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
# <a name="unable-to-enable-unified-auditing"></a>Det går inte att aktivera enhetlig granskning

NÃ¤r du fÃ¶rsÃ¶k fÃ¶rsÃ¶k att aktivera enhetlig granskning fÃ¶r din organisation kan ett felmeddelande visas fÃ¶rsÃ¶k:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Så här löser du problemet:

1. [Anslut till Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Kör följande cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Vänta i 60 minuter innan den föregående inställningen börjar gälla.

4. Kör följande kommando i Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Mer information finns i följande artiklar:

- [Ansluta till Exchange Online PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Aktivera och inaktivera granskningsloggsökning](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
