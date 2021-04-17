---
title: Prenumerationstyper som stöds
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
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820700"
---
# <a name="supported-subscription-types"></a>Prenumerationstyper som stöds

Granska vilka prenumerationstyper som stöds för att gå vidare.

[Prenumerationstyper som stöds](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Överför faktureringsägarskap**

Azure Portal som [Kontoadministratör](https://ms.portal.azure.com/) för det faktureringskonto som har den prenumeration du vill överföra.

- Sök på **Kostnadshantering + fakturering**. Välj **Prenumerationer** från den vänstra rutan. Beroende på åtkomst kan du behöva välja ett faktureringsomfång och sedan **Prenumerationer** eller **Azure-prenumerationer**.
- Välj Överför faktureringsägarskap för den prenumeration du vill överföra.
- Ange e-postadressen till en användare som är faktureringsadministratör för kontot som kommer att bli den nya ägaren för prenumerationen och välj sedan **Skicka begäran om överföring**.
- Användaren får ett e-postmeddelande med instruktioner för att granska din överföringsbegäran. Om du vill godkänna överföringsbegäran väljer användaren länken i e-postmeddelandet och följer anvisningarna.

Tänk på att om du överför faktureringsägarskapet för prenumerationen till ett användarkonto i en annan Azure AD-klientorganisation, tas alla uppgifter för [rollbaserad åtkomstkontroll (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) för att hantera resurser i prenumerationen bort permanent. Det är bara den nya ägaren som får åtkomst till hantering av resurser i prenumerationen. Om du vill ha mer information kan du läsa [Överföra prenumeration till en användare i en annan Azure AD-klientorganisation](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Överföra ägarskap för prenumeration**

Överföring av ägarskap för prenumeration förutsätter rollbaserad åtkomstkontrollsroll (RBAC) för att hantera resurser i prenumerationen, de som hade den rollen förlorar åtkomsten vid överföringen. Mer information om hur du lägger till en befintlig prenumeration för en klientorganisation finns i [Koppla eller lägga till en Azure-prenumeration i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Prenumerationsöverföring med ett befintligt utestående belopp från den aktuella faktureringsperioden överförs inte till det nya betalningsinstrumentet på det nya kontot. Den enda information som är tillgänglig för användarna på det nya kontot är den senaste månadens kostnad för prenumerationen. Resten av användnings- och faktureringshistoriken överförs inte med prenumerationen.
- Överföra faktureringsägarskap för prenumerationer av Enterprise-avtal (EA) stöds för närvarande endast i portalen för Enterprise-avtal
- För att en ny användare ska kunna acceptera en överföringsbegäran på kreditinriktade prenumerationer som Visual Studio, BizSpark och Microsoft Partner Network, behövs en Visual Studio/Microsoft Partner Network-licens
- Alla resurser som Virtual Machines, diskar och webbplatser överförs till det nya kontot. Följande resurser kan påverkas i en prenumerationsöverföring mellan klientorganisationer:

**Azure AD Domain Services**

Azure Key Vaults

- [SQL-relaterade användare och databaser](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support)kan påverkas, särskilt om kunden använder en Azure Active Directory-relaterad autentisering
- **App-tjänster** som är konfigurerade med Azure Active Directory-autentisering kan påverkas
- **Visual Studio Team**-tjänstkonton som är anslutna till Azure-prenumerationer kan tillfälligt förlora åtkomst när den anslutna Azure-prenumerationen avbryts

**Rekommenderade dokument**

Steg efter att du har accepterat faktureringsägarskap:

- Om du vill behålla faktureringsägarskap men ändra typen, läs: [Ändra din Azure-prenumeration till ett annat erbjudande](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Överföring av utvecklings-/testprenumerationer för Visual Studio, Microsoft Partner Network (MPN) och Betala per användning](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Överföra faktureringsägarskap för prenumerationer av Enterprise-avtal (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Vanliga frågor och svar om överföring av ägarskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Felsöka problem med överföring av ägarskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)