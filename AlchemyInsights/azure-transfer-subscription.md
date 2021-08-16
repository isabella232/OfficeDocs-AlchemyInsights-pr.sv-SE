---
title: Överför Azure faktureringsägarskap
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
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036114"
---
# <a name="transfer-azure-billing-ownership"></a>Överför Azure faktureringsägarskap

Logga in på [Azure-portalen](https://portal.azure.com/) som administratör för det faktureringskonto som har den prenumeration du vill överföra. Om du är osäker på om du är-administratör, eller om du behöver bestämma vem som är det, läser du[Avgör konto för fakturerings administratör](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Sök på _Kostnadshantering + fakturering_.
1. Välj **Prenumerationer** från den vänstra rutan. Beroende på åtkomst kan du behöva välja en faktureringsomfång och sedan **Prenumerationer** eller **Azure-prenumerationer**.
1. Välj **Överför faktureringsägarskap** för den prenumeration du vill överföra.
1. Ange e-postadressen till en användare som är faktureringsadministratör för kontot som kommer att bli den nya ägaren för prenumerationen och välj sedan **Skicka begäran om överföring**.
1. Användaren får ett e-postmeddelande med instruktioner för att granska din överföringsbegäran. Om du vill godkänna överföringsbegäran väljer användaren länken i e-postmeddelandet och följer anvisningarna.

Tänk på att om du överför faktureringsägarskap för prenumerationen till en användarkonto i en annan Azure AD-klient organisation, tas alla [rollbaserad åtkomstkontroll (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) uppgifter för att hantera resurser i prenumerationen bort permanent. Det är bara den nya ägaren som får åtkomst till hantering av resurser i prenumerationen. Om du vill ha mer information om hur du ändrar katalog för en-prenumeration kan du läsa [Överföra prenumeration till en användare i en annan Azure AD-klient organisations](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Viktigt påverkan på dina fakturor**_: om du har överfört faktureringsägarskap för en Azure-prenumeration kommer dina kostnader att bli proportionella. Du kan komma åt fakturorna enligt följande:  

1. Välj din prenumeration på sidan [Prenumerationer](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i Azure-portalen som [en användare med åtkomst till fakturor](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)och välj **Fakturor**.
1. Klicka på **Hämta faktura** för att visa en kopia av PDF-fakturan. Om det står _Inte tillgänglig_ läser du [Varför ser jag ingen faktura för den senaste faktureringsperioden?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Du kan också visa din dagliga användning genom att klicka på den **faktureringsperioden** för att få en PDF-fil med fakturan och en kopia av din detaljerade dagliga användning fil (.CSV). Mer information finns i [Få fakturan-och användnings data](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Rekommenderade dokument**

- [Överföra faktureringsägarskap för en Azure-prenumeration till ett annat konto](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Om överföring av faktureringsägarskap för en Azure-prenumeration](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Överföring av Visual Studio, Microsoft Partner Network (MPN)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Vanliga frågor och svar om överföring av ägarskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Felsöka problem med överföring av ägarskap](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
