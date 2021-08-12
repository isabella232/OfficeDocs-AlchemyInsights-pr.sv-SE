---
title: Återställa borttagna objekt med cmdlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: b3f4f034d5d7486dafa1b5c1801a285b09a34644b811146f09f454fad9647833
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910672"
---
# <a name="recover-deleted-items-with-cmdlet"></a>Återställa borttagna objekt med cmdlet

- Använd cmdleten [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) för att visa borttagna objekt i postlådor. När du har hittat de borttagna objekten använder du cmdleten [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) för att återställa dem.

- Se fullständig information i [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).

- Du måste vara tilldelad rollen Importera och exportera postlåda innan du kan köra den här cmdleten. Mer information finns i [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).
