---
title: Lägga till och hantera administratörer – rekommenderade steg
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
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963805"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Lägga till och hantera administratörer – rekommenderade steg

Baserat på din problembeskrivning har vi hittat en lösning åt dig. De flesta kunder kunde lösa problemet på egen hand efter att ha följt vår dokumentation.

**Redigera prenumerationsadministratören eller medadministratören**

- Kontoadministratören kan redigera båda rollerna medan prenumerationsadministratören bara kan ändra medadministratörer i [Azure-portalen.](https://ms.portal.azure.com/#home)
- [Lägga till eller ändra Azure-prenumerationsadministratörer](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Uppdatera prenumerationsadministratören eller Co-Administrator för interna (AIRS) prenumerationer**

Tjänstadministratören eller medadministratören kan själv använda den här åtgärden på följande sätt:

1. Logga in på [Azure-portalen och](https://ms.portal.azure.com/#home) klicka **på Kostnadshantering + Fakturering** i det vänstra bladet.
2. Klicka på radobjektet för din prenumeration. Då öppnas Översikt för din prenumeration.
3. Klicka på **Egenskaper** i **prenumerationsbladet.** 
4. Klicka på **knappen Tjänstadministratör.**
5. Ange e-postadressen till den användare som du vill ange som tjänstadministratör och klicka på **OK.**

**Lägg till/ändra/ta bort medadministratör**

1. Logga in på [Azure Portal som](https://ms.portal.azure.com/#home) tjänstadministratör.
2. Öppna [Prenumerationer](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) och välj en prenumeration. (Medadministratörer kan bara tilldelas prenumerationen.)
3. Gå till Den klassiska administratören för **Access-kontroller (IAM)** Lägg till medadministratör för att öppna fönstret Lägg till medadministratör (om alternativet Lägg till med administratör är inaktiverat betyder det att du inte har  >    >    >   behörighet). 
4. Markera den användare som du vill lägga till och klicka på **Lägg till.**

**Lära sig mer:**
- [Lägga till en medadministratör](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ta bort en medadministratör](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ändra tjänstadministratör](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Visa kontoadministratören](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Hantera åtkomst med RBAC och Azure Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Lägga till/ta bort användare med Azure Active Directory (AD)**

Du kan lägga till nya användare eller ta bort befintliga användare från Azure Active Directory -organisationen (Azure AD):

1. Om du vill lägga till en ny användare loggar du in [på Azure](https://ms.portal.azure.com/#home) Portal som en användaradministratör för organisationen.
2. Välj **Azure Active Directory**, välj **Användare och** klicka sedan på Ny **användare.**
3. Fyll **i den** information som krävs på sidan Användare. Klicka på **Skapa**. Användaren skapas och läggs till i Azure AD-klienten.

**Läs mer:**

- [Lägga till en ny användare](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Ta bort en användare](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Lägga till eller uppdatera en användares profilinformation med hjälp av Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Rekommenderade dokument**

- [Vad är rollbaserad åtkomstkontroll (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Förstå de olika rollerna i Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administratörens rollbehörigheter i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Självstudiekurs: Bevilja åtkomst för en användare med RBAC och Azure Portal](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Felsöka RBAC i Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Ordna dina resurser med Azure-hanteringsgrupper](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Så här begär du en kopia av Azure-faktura via e-post](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Lägga till, uppdatera eller ta bort ett kreditkort eller betalkort från Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Hantera (Återaktivera/Avbryt/Byt)-prenumeration](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



