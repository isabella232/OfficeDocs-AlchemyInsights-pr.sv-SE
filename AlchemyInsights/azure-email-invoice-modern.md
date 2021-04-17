---
title: Modern e-postfakturering i Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820844"
---
# <a name="email-invoicing-in-azure"></a>E-postfakturering i Azure

Du måste ha en ägar- eller en deltagarroll i faktureringsprofilen eller det tillhörande faktureringskontot för att kunna uppdatera inställningen för e-postfakturering. När du har anmält dig får alla användare med en ägar-, deltagar-, läsar- och fakturahanteringsroller i en faktureringsprofil fakturan via e-post.

1. Logga in på [Azure-portalen](https://portal.azure.com/).
2. Sök på **Kostnadshantering + fakturering**.
3. Välj **Fakturor** på den vänstra sidan och välj sedan **E-postfaktura** högst upp på sidan.
4. Om du har flera faktureringsprofiler väljer du en faktureringsprofil och väljer sedan **Anmäl dig**.

5. Välj **Uppdatera**.
6. Om du har flera faktureringsprofiler markerar du en faktureringsprofil och väljer sedan **Anmäl dig**.

Du ger andra tillgång till att visa, ladda ned och betala fakturor genom att tilldela dem rollen som fakturahanterare för en MCA- eller MPA-faktureringsprofil. Om du har valt att hämta fakturan via e-post får även användarna sina fakturor via e-post.

1. Logga in på [Azure-portalen](https://portal.azure.com/).
2. Sök på **Kostnadshantering + fakturering**.
3. Markera **Faktureringsprofiler** på den vänstra sidan. Markera en faktureringsprofil i listan med faktureringsprofiler som du vill tilldela en fakturahanteringsroll.
4. Markera **Åtkomstkontroll (IAM)** på den vänstra sidan och markera sedan **Lägg till** högst upp på sidan.

I listrutan Roll markerar du **Fakturahanterare**. Ange användarens e-postadress för att ge åtkomst. Markera **Spara** för att tilldela rollen.
