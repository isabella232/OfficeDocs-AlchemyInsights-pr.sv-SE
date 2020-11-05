---
title: Moderna Azure e-postfakturering
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922145"
---
# <a name="email-invoicing-in-azure"></a>E-postfakturering i Azure

Du måste ha en ägare eller deltagar roll i fakturerings profilen eller dess fakturerings konto för att kunna uppdatera e-postfakturans preferens. När du har valt det får alla användare med rollerna ägare, deltagare, läsare och faktura chef i en fakturerings profil sin faktura via e-post.

1. Logga in på [Azure-portalen](https://portal.azure.com/).
2. Sök efter **kostnads hantering + fakturering**.
3. Välj **fakturor** till vänster och välj sedan **e-postfaktura** längst upp på sidan.
4. Om du har flera fakturerings profiler väljer du en fakturerings profil och väljer sedan **opt in**.

5. Välj **Uppdatera**.
6. Om du har flera fakturerings profiler väljer du en fakturerings profil och väljer sedan **opt in**.

Du ger andra till gång till Visa, ladda ned och betala fakturor genom att tilldela dem rollen som faktura chef för en betalnings profil för MCA eller MPA. Om du har valt att få fakturan i ett e-postmeddelande får användarna också fakturor via e-post.

1. Logga in på [Azure-portalen](https://portal.azure.com/).
2. Sök efter **kostnads hantering + fakturering**.
3. Välj **betalnings profiler** från vänster sida. I listan betalnings profiler väljer du en betalnings profil som du vill tilldela en faktura administratörs roll.
4. Välj **åtkomst kontroll (IAM)** från den vänstra sidan och välj sedan **Lägg till** högst upp på sidan.

I list rutan Role väljer du **faktura chef**. Ange e-postadressen för den användare som ska ge åtkomst. Välj **Spara** för att tilldela rollen.
