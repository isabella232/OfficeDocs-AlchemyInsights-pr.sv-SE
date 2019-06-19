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
# <a name="unable-to-enable-unified-auditing"></a>Det går inte att aktivera enhetlig granskning

När du försöker aktivera enhetlig granskning för organisationen Office 365 kan du få ett felmeddelande liknande följande:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Lös problemet så här:

1. [Ansluta till Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Kör du följande cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Vänta i 60 minuter för den tidigare inställningen ska börja gälla.

4. Kör följande kommando i Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Mer information finns i följande artiklar:

- [Ansluta till Exchange Online PowerShell använder autentisering i flera steg](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Aktivera och inaktivera Office 365 Granska loggen Sök](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
