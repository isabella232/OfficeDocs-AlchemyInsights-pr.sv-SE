---
title: 2419-det går inte att aktivera-granskning
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767617"
---
# <a name="unable-to-enable-unified-auditing"></a>Det går inte att aktivera enhetlig granskning

När du försöker aktivera enhetlig granskning för din organisation kan du få ett fel av följande slag:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Lös problemet genom att följa de här stegen:

1. [Anslut till Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Kör följande cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Vänta till 60 minuter innan föregående inställning börjar gälla.

4. Kör följande kommando i Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Mer information finns i följande artiklar:

- [Ansluta till Exchange Online PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Aktivera och inaktivera granskningsloggsökning](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
