---
title: Överför ägandes Kap för Azure
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922171"
---
# <a name="transfer-azure-billing-ownership"></a>Överför ägandes Kap för Azure

Logga in på [Azure-portalen](https://portal.azure.com/) som administratör för det fakturerings konto som har den prenumeration du vill överföra. Om du är osäker på om du är och administratör, eller om du behöver ta reda på vem som är, kan du läsa [kontrol lera konto fakturerings administratör](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Sök på **kostnads hantering + fakturering**.
- Välj **prenumerationer** från vänster fönster ruta. Beroende på åtkomst kan du behöva välja en fakturerings omfattning och sedan **prenumerationer** eller **Azure-prenumerationer**.
- Välj **överför ägandes Kap** för abonnemanget som du vill överföra
- Ange e-postadressen för en användare som är fakturerings administratör för det konto som kommer att bli den nya ägaren för abonnemanget och sedan välja **Skicka överförings förfrågan**
- Användaren får ett e-postmeddelande med instruktioner för att kontrol lera din överföringsbegäran. För att godkänna överföringsbegäran väljer användaren länken i e-postmeddelandet och följer anvisningarna.

**Obs!** om du överför fakturerings ägandet för ditt abonnemang till en användares konto i en annan Azure AD-klient organisation, tas alla aktiviteter för [rollbaserad åtkomst kontroll (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)för att hantera resurser i prenumerationen permanent bort. Endast den nya ägaren får åtkomst till att hantera resurser i prenumerationen. Mer information finns i [överföra ett abonnemang till en användare i en annan Azure AD-klient organisation](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Rekommenderade dokument**

- [Överföra fakturerings ägandes Kap för ett Azure-abonnemang till ett annat konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Om att överföra ägandes Kap till en Azure-prenumeration](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Överför Visual Studio, Microsoft Partner Network (MPN) och betala allt eftersom med prov abonnemang](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Vanliga frågor och svar om ägarskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Felsöka problem med överförings ägarskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
