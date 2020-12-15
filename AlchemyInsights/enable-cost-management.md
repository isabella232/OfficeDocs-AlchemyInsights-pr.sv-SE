---
title: Aktivera kostnads hantering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678773"
---
# <a name="enable-cost-management"></a>Aktivera kostnads hantering

**Vad innebär "kostnaderna är inaktiverade för din organisation"?**

Organisationer som använder Enterprise Agreement (EA) eller Microsoft Customer Agreement (MCA)-konton kan förhindra åtkomst till information om kostnader och priser.

När du har loggat in på Azure Portal kan de använda API-gränssnitten för att programmatiskt skaffa fakturor (när du har valt) och användnings uppgifter.

**Så här tillåter du fler användare att få åtkomst till fakturor**

1. Gå till **prenumerationens blad** i Azure Portal.
2. Välj **fakturor** och sedan **åtkomst till fakturor**.
3. Aktivera åtkomst och följ sedan de ändringar du vill göra för att tillåta användare i prenumerations bara roller att ladda ner fakturor.

> [!NOTE]
> Konto administratören kan också konfigurera så att fakturor skickas via e-post. Mer information finns i [Hämta din faktura via e-post](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Så här lägger du till användare i rollen fakturerings läsare**

1. Gå till **prenumerationens blad** i Azure Portal.
2. Välj **åtkomst kontroll (IAM)** och klicka sedan på **Lägg till**.
3. Välj **fakturerings läsare** på sidan **Välj en roll** .
4. Skriv e-postmeddelandet för den användare som du vill bjuda in och klicka sedan på **OK** för att skicka inbjudan.
5. Följ instruktionerna i inbjudan via e-post om du vill logga in som en fakturerings läsare. Mer information finns i [bevilja åtkomst till fakturering](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Rekommenderade dokument**

- [Aktivera DA-och AO-vyer via EA-portalen](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kostnader inkluderade i kostnads hantering](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Support för Microsoft Azure](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Granska kostnader i kostnads analys](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Ge åtkomst till fakturerings uppgifter](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kontrol lera åtkomsten till ett Microsoft-kundavtal](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






