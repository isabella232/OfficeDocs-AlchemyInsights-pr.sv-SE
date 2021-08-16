---
title: Migrering från AIP till MIP/Unified Labeling i efterlevnadscentret
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
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000384"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrering från AIP till MIP/Unified Labeling i efterlevnadscentret

Så här migrerar du från AIP-etiketter till Unified Labeling i Säkerhets- och efterlevnadscenter:

**Aktivera skydd från Azure Portal**

1. Om du inte redan har gjort det öppnar du ett nytt webbläsarfönster och [loggar in på Azure Portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Gå till **bladet för Azure Information Protection.** I till exempel hubb-menyn klickar du **på Alla tjänster** och börjar skriva **Information** i rutan Filter. Välj **Azure Information Protection**. Om du inte har åtkomst till Azure Information Protection-bladet tidigare kan du gå till de ytterligare anvisningarna [för](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) att lägga till det här bladet i portalen. För att kunna öppna Azure Information Protection-bladet måste du ha ett [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller ett Office 365 som omfattar Rättighetshantering. Om du har en av dessa prenumerationer men ser ett meddelande om att det inte går att hitta en giltig prenumeration kontaktar du [Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller använder dina standardsupportkanaler.

2. Leta reda **på** menyalternativen Hantera och välj **Skyddaktivering**. Klicka **på** Aktivera och bekräfta sedan åtgärden. När aktiveringen är klar visas aktiveringen **som slutförd i informationsfältet.**

**Migrera Azure Information Protection-etiketter Office 365 säkerhets- & efterlevnadscenter**

1. Kontrollera att du är inloggad som användare med behörigheten Global administratör.

2. Gå till **bladet för Azure Information Protection.**

3. I **menyalternativet** Hantera väljer du **Unified Labeling**.

4. I Azure **Information Protection – enhetligt etikettblad klickar** du på Aktivera **och** följer onlineinstruktionerna.

**Obs!** Kontrollera att du har rätt behörigheter innan du aktiverar migreringen av säkerhets- & säkerhets- och efterlevnadscentret. Mer information finns i följande artiklar:

1. [Behöver du vara global administratör för att konfigurera Azure Information Protection, eller kan jag delegera till andra administratörer?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Viktig information om administrativa roller efter migrering till Säkerhets- & Efterlevnadscenter.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Mer information om migrering av AIP till Unified Labeling till Säkerhets- och efterlevnadscenter finns i [Migrera etiketter.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
