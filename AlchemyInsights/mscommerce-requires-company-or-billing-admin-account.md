---
title: Ansluta till MSCommerce-modulen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 80735a03eef6ef9f7b791c43019678ea01f83c00
ms.sourcegitcommit: 9db3be25d088b8d4b2d476aeace79e653ca0a421
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/17/2020
ms.locfileid: "42093640"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce kräver ett företags- eller faktureringsadministratörskonto

MSCommerce-modulen kräver ett konto med företags- eller faktureringsadministratörsbehörighet. Om du får följande fel måste du återansluta till ett annat konto.

    ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - 
    At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5
    +     HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...
    +     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        + CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException
        + FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError

Om ditt konto inte har företags- eller faktureringsadministratörsbehörighet kontaktar du IT-administratören.
