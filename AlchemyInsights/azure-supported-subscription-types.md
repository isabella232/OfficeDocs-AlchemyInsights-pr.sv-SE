---
title: Abonnemangs typer som stöds
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
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807981"
---
# <a name="supported-subscription-types"></a>Abonnemangs typer som stöds

Granska de abonnemangs typer som stöds för att fortsätta.

[Abonnemangs typer som stöds](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Överför ägandes Kap**

Azure-portalen som [konto administratör](https://ms.portal.azure.com/) för det fakturerings konto som har den prenumeration du vill överföra

- Sök på **kostnads hantering + fakturering** . Välj **prenumerationer** från vänster fönster ruta. Beroende på åtkomst kan du behöva välja en fakturerings omfattning och sedan **prenumerationer** eller **Azure-prenumerationer** .
- Välj överför ägandes Kap för abonnemanget som du vill överföra
- Ange e-postadressen för en användare som är fakturerings administratör för det konto som kommer att bli den nya ägaren för abonnemanget och sedan välja **Skicka överförings förfrågan**
- Användaren får ett e-postmeddelande med instruktioner för att kontrol lera din överföringsbegäran. För att godkänna överföringsbegäran väljer användaren länken i e-postmeddelandet och följer anvisningarna.

Obs! Om du överför fakturerings ägandet för ditt abonnemang till en användares konto i en annan Azure AD-klient organisation, tas alla aktiviteter för [rollbaserad åtkomst kontroll (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) för att hantera resurser i prenumerationen permanent bort. Endast den nya ägaren får åtkomst till att hantera resurser i prenumerationen. Mer information finns i [överföra ett abonnemang till en användare i en annan Azure AD-klient organisation](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Överför Ägandes Kap för abonnemang**

Abonnemangs ägarskap överföring för nödvändiga roller baserad åtkomst (RBAC) för att hantera resurser i prenumerationen förlorar deras åtkomst. Mer information om hur du lägger till befintliga abonnemang i en klient organisation finns i [associera eller lägga till en Azure-prenumeration i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Abonnemangs överföring med ett befintligt utestående belopp från den aktuella debiterings perioden överförs inte till det nya betalnings instrumentet i det nya kontot. Den enda tillgängliga informationen för användarna på det nya kontot är den senaste månadens kostnad för ditt abonnemang. Resten av användnings-och fakturerings historiken överförs inte med abonnemanget.
- Överföring av fakturerings ägandes Kap för Enterprise Agreement-prenumerationer (EA) stöds för närvarande endast i Enterprise Agreement-portalen
- Att överföra ett kundorienteradt abonnemang som Visual Studio, BizSpark, Microsoft Partner Network till en ny användare måste ha en Visual Studio/Microsoft Partner Network-licens för att acceptera överföringsbegäran
- Alla resurser som virtuella datorer, diskar och webbplatser överförs till det nya kontot. Följande resurser kan påverkas av en prenumeration på flera innehavare:

**Azure AD Domain Services**

Azure Key-valv

- [SQL-relaterade användare och databaser](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) kan påverkas, särskilt om kunden använder en Azure Active Directory-relaterad verifikation
- **Program tjänster** som har kon figurer ATS med Azure Active Directory-auktorisering kan påverka
- **Visual Studio-teamet** Tjänster som är anslutna till Azure-prenumerationer kan tillfälligt förlora åtkomst när det anslutna Azure-abonnemanget avbryts

**Rekommenderade dokument**

Steg efter att du har accepterat fakturerings ägandet:

- Om du vill behålla fakturerings ägandet men ändra typen för ditt abonnemang kan du läsa: [byta ditt Azure-abonnemang till ett annat erbjudande](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Överför Visual Studio, Microsoft Partner Network (MPN) och betala allt eftersom med prov abonnemang](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Överföra fakturerings ägandes Kap för Enterprise Agreement (EA)-abonnemang](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Vanliga frågor och svar om ägarskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Felsöka problem med överförings ägarskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)