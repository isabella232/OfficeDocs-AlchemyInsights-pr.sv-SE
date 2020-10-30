---
title: Åtkomst till prenumeration
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807723"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Det går inte att logga in i Azure på grund av webbläsarens problem (webbläsaren hänger sig, fungerar inte, laddas inte osv.)

Du kan ha drabbats av ett avbrott. Kontrol lera om det finns ett pågående avbrott: [Azure Health status](https://status.azure.com/status/history/).

Logga ut från alla aktiva Azure-sessioner. Starta ett privat eller inkognitofönstert läge i webbläsaren.

Du kan också försöka uppdatera webbläsaren, använda en annan webbläsare och ta bort cache-cookies om ovanstående inte fungerar.

Läs mer: [Felsöka inloggnings problem](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Det går inte att komma åt abonnemang**

I [Azure-portalen](https://portal.azure.com/)kontrollerar du att rätt Azure-katalog är vald från kontot längst upp till höger.

I [Azure-konto Center](https://account.windowsazure.com/Subscriptions)kontrollerar du att det konto som används är konto administratören.

Läs mer: [Felsöka inga prenumerationer](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Kunde inte komma åt fakturerings historik**

Konto administratören måste kontrol lera att användaren som använder fakturerings informationen läggs till i Azure Active Directory som gäst användare: [lägga till eller ta bort en ny användare](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Användaren måste då ges rollen som global administratör: [tilldela användare rollen](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Publicera detta kan användaren få till gång till en debiterings åtkomst med RBAC-principer: [bevilja åtkomst till fakturering](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Rekommenderade dokument**

-   [Jag kan inte logga in för att hantera mitt Azure-abonnemang](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)