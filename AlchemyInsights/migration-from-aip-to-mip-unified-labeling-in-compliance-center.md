---
title: Migrering från AIP till MIP/Unified-etiketter i Compliance Center
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674344"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrering från AIP till MIP/Unified-etiketter i Compliance Center

Om du vill migrera från AIP Labels till Unified Etiketting i säkerhets-och kompatibilitetstillstånd gör du så här:

**Aktivera skydd från Azure-portalen**

1. Om du inte redan har gjort det öppnar du ett nytt webbläsarfönster och loggar in på [Azure-portalen](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Navigera till bladet **Azure information Protection** . Klicka till exempel på **alla tjänster** på NAV-menyn och börja skriva in **information** i rutan filter. Välj **Azure information Protection**. Om du inte har fått åtkomst till bladet Azure information Protection innan kan du se de enskilda [åtgärderna](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) för att lägga till bladet i portalen. Om du vill öppna Azure information Protection-bladet måste du ha ett [Azure information Protection Premium-abonnemang](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller ett Office 365-abonnemang som innehåller Rights Management. Om du har en av de här prenumerationerna men ser ett meddelande om att det inte går att hitta ett giltigt abonnemang [kontaktar du Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller använder dina Standard Support kanaler.

2. Leta reda på Meny alternativen **Hantera** och välj **skydds aktivering**. Klicka på **Aktivera**och bekräfta åtgärden. När aktiveringen är färdig visar informations fältet **aktiveringen klar**.

**Migrera Azure information Protection-etiketter till Office 365 Security & Compliance Center**

1. Kontrol lera att du är inloggad som en användare med global administratörs behörighet.

2. Navigera till bladet **Azure information Protection** .

3. Välj **Unified etiketting**i menyn **Hantera** .

4. På sidan **Azure information Protection-enhetligt etikett** blad klickar du på **Aktivera** och följer instruktionerna online.

**Obs!** kontrol lera att du har rätt behörighet innan du aktiverar säkerhets &s Center migration. Mer information finns i de här artiklarna:

1. [Måste du vara global administratör för att konfigurera Azure information Protection eller kan jag delegera till andra administratörer?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Viktig information om administrativa roller efter migrering till säkerhets & Compliance Center.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Mer information om AIP till enhetlig etikett överföring till säkerhets-och efterlevnadsprinciper finns i [migrera etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
