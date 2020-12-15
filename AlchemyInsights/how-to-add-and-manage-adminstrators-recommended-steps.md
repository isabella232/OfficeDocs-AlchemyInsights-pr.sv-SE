---
title: Så här lägger du till och hanterar adminstrators – rekommenderade steg
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678870"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Så här lägger du till och hanterar adminstrators – rekommenderade steg

**Redigera abonnemangs administratören eller medadministratören**

- Konto administratören kan redigera båda rollerna och abonnemangs administratören kan bara ändra samarbets administratörer i [Azure-portalen](https://ms.portal.azure.com/#home).
- [Lägga till eller ändra Azure-prenumerationens administratörer](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Uppdatera abonnemangs administratören eller Co-Administrator för interna (översändnings-) abonnemang**

Tjänst administratören eller medarbetaren kan själv hantera den här åtgärden genom att utföra följande steg:

1. Logga in på [Azure-portalen](https://ms.portal.azure.com/#home) och klicka på **kostnads hantering + fakturering** i det vänstra bladet.
2. Klicka på rad posten med ditt abonnemang. Då öppnas översikten för din prenumeration.
3. Klicka på **Egenskaper** i **prenumerations** bladet. 
4. Klicka på knappen **tjänst administratör** .
5. Ange e-postmeddelandet för den användare som du vill ange som tjänst administratör och klicka på **OK**.

**Lägga till/ändra/ta bort administratör**

1. Logga in på [Azure-portalen](https://ms.portal.azure.com/#home) som tjänst administratör.
2. Öppna [abonnemang](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) och välj ett abonnemang. (Co-adminstrators kan bara tilldelas i prenumerations omfattningen.)
3. Navigera till **åtkomst kontroll (IAM)**  >  **klassiska administratörer** lägga till en administratör  >    >   för att öppna fönstret **Lägg till** medarbetaren (om alternativet för att lägga till medarbetaren är inaktiverat) anger det att du inte har behörighet.
4. Välj den användare som du vill lägga till och klicka på **Lägg till**.

**Lära sig mer:**
- [Lägga till en administratör för administratörer](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ta bort en administratör för administratörer](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ändra tjänstens administratör](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Visa konto administratören](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Hantera åtkomst med RBAC och Azure Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Lägga till/ta bort användare med Azure Active Directory (AD)**

Du kan lägga till nya användare eller ta bort befintliga användare från din Azure Active Directory (Azure AD)-organisation:

1. Om du vill lägga till en ny användare loggar du in på [Azure-portalen](https://ms.portal.azure.com/#home) som en användares administratör för organisationen.
2. Välj **Azure Active Directory**, Välj **användare** och klicka sedan på **ny användare**.
3. Fyll i informationen på sidan **användare** . Klicka på **Skapa**. Användaren skapas och läggs till i din Azure AD-klient.

**Läs mer**:

- [Lägga till en ny användare](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Ta bort en användare](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Lägga till eller uppdatera en användares profil information med Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Rekommenderade dokument**

- [Vad är rollbaserad åtkomst kontroll (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Förstå de olika rollerna i Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administratörens rollbehörigheter i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Själv studie kurs: bevilja åtkomst för en användare med RBAC och Azure-portalen](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Felsöka RBAC i Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Ordna dina resurser med Azure Management Groups](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Så här efterfrågar du kopia av en Azure-faktura via e-post](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Lägga till, uppdatera eller ta bort ett kredit-eller betalkort från Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Hantera (återaktivera/Avbryt/byta) abonnemang](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



