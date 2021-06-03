---
title: Skicka in en hårddisk Microsoft 365 importtjänsten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731949"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Skicka in en hårddisk Microsoft 365 importtjänsten

Använd skicka in en hårddisk genom att kopiera PST-filer till en hårddisk och sedan skicka hårddisken till Microsoft.

Så här startar du jobbet:

1. Välj Microsoft 365 i **kompatibilitetscentret** under **Informationsstyrning.**

1. Välj **Välj importjobbtyp** och välj sedan **Nästa.**

1. För att se stegen för det här importalternativet **väljer du Ship hard drives to one of our physical locations**.

Här är några saker att tänka på:

- Du måste vara tilldelad rollen Importera och exportera postlåda i Exchange Online kunna importera PST-filer till Microsoft 365 postlådor.
Prestanda kan påverkas för PSTs som är större än 20 GB.

- Endast 2,5-tums SSD (Solid-state Drives) eller 2,5- eller 3,5-tums SATA II/III interna hårddiskar stöds.
Hårddisken som innehåller PST-filer måste krypteras med BitLocker.

- Kostnaden för att importera PST-filer Microsoft 365 postlådor som använder leverans är 2 USD per GB data.

Mer information om hur du använder metoden för att skicka in en hårddisk för att importera PST-filer finns i Använda möjligheten att skicka in en hårddisk för [att importera organisationens PST-filer.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)