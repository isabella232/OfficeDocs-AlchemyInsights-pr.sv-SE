---
title: Prenumerationsåtkomst
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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999258"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Det går inte att logga in i Azure på grund av problem med webbläsaren (webbläsaren hänger sig, snurrar, läses inte in osv.)

Du kan påverkas av ett avbrott. Kontrollera om det är pågående avbrott: [Azure Health Status](https://status.azure.com/status/history/).

Logga ut från alla aktiva Azure-sessioner. Starta ett privat eller inkognitoläge i webbläsaren.

Du kan också prova att uppdatera webbläsaren, använda en annan webbläsare, ta bort cachekakor om ovanstående inte fungerar.

Läs mer: [Felsöka inloggningsproblem](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Det går inte att komma åt prenumerationer**

Kontrollera att [rätt Azure-katalog](https://portal.azure.com/)har valts i kontot längst upp till höger i Azure-portalen.

I [Azure-kontocentret](https://account.windowsazure.com/Subscriptions)ser du till att det konto som används är kontoadministratör.

Läs mer: [Felsöka Inga prenumerationer hittades](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Det går inte att komma åt faktureringshistoriken**

Kontoadministratören måste se till att användaren som har åtkomst till faktureringsinformationen läggs till i Azure Active Directory som gästanvändare: Lägga till eller ta [bort en ny användare.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Användaren måste sedan ges rollen Global administratör: Tilldela [roll till användare](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Efter detta kan användaren få faktureringsåtkomst med principer för RBAC: [Bevilja åtkomst till fakturering.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Rekommenderade dokument**

-   [Jag kan inte logga in för att hantera min Azure-prenumeration](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)