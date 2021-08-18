---
title: Aktivera kostnadshantering
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
ms.openlocfilehash: 62f3cfb161c4f8da735bd288a2d6e22971b4aada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325481"
---
# <a name="enable-cost-management"></a>Aktivera kostnadshantering

**Vad innebär "kostnader inaktiveras för din organisation"?**

Organisationer som använder företagsavtal (EA) eller Microsofts kundavtalskonton (MCA) kan inaktivera åtkomst till kostnadsinformation och prisinformation.

När de har loggat in på Azure Portal kan de använda fakturerings-API:er för att programmässigt få fakturor (när de har valt) och användningsinformation.

**Så här tillåter du att ytterligare användare får åtkomst till fakturor**

1. Gå till **Prenumerationsblad** i Azure Portal.
2. Välj **Fakturor** och välj **sedan Åtkomst till fakturor.**
3. Aktivera åtkomsten, följt av att spara ändringarna, så att användare i prenumerationsbaserade roller kan hämta fakturor.

**Obs!** Kontoadministratören kan också konfigurera så att fakturor skickas via e-post. Mer information finns i Hämta [din faktura via e-post.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)

**Lägga till användare i rollen Faktureringsläsare**

1. Gå till **Prenumerationsblad** i Azure Portal.
2. Välj **Åtkomstkontroll (IAM) och** klicka sedan på Lägg **till**.
3. Välj **Faktureringsläsare** på **sidan Välj en** roll.
4. Skriv e-postadressen till den användare som du vill bjuda in och klicka sedan **på OK för** att skicka inbjudan.
5. Följ anvisningarna i e-postmeddelandet för inbjudan för att logga in som en faktureringsläsare. Mer information finns i [Bevilja åtkomst till fakturering.](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)

**Rekommenderade dokument**

- [Aktivera DA- och AO-vyer via EA-portalen](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kostnader som ingår i Kostnadshantering](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Support Microsoft Azure erbjudanden](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Granska kostnader i kostnadsanalyser](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Ge åtkomst till faktureringsinformation](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kontrollera åtkomst till ett Microsoft-kundavtal](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






