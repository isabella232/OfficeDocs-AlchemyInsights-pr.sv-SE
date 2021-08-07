---
title: 'RBAC-roller '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923149"
---
# <a name="rbac-rules"></a>RBAC-regler

Om du får behörighetsfelet: 

- Klienten med objekt-ID har ingen auktorisering för att utföra åtgärder över omfattningen **(kod: AuthorizationFailed)**: när du försöker skapa en resurs kontrollerar du att du är inloggad med en användare som har tilldelats en roll som har skrivbehörighet till resursen i den valda omfattningen. Om du till exempel vill hantera virtuella datorer i en resursgrupp bör du ha rollen [Deltagare](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) för virtuell dator i resursgruppen (eller överordnad omfattning). En lista över behörigheterna för varje inbyggd roll finns i [Inbyggda roller för Azure-resurser.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Du har inte behörighet att skapa en **supportbegäran:** när du försöker skapa eller uppdatera ett supportbegäran ska du kontrollera att du är inloggad med en användare [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)som har tilldelats en roll som har behörigheten Microsoft.Support/supportTickets/write, till exempel deltagare i supportbegäran.
- Du kan inte skapa fler rolltilldelningar **(kod: RoleAssignmentLimitExceeded):** När du försöker tilldela en roll bör du försöka minska antalet rolltilldelningar genom att tilldela roller till grupper i stället. Azure har stöd för **upp till 2 000** rolltilldelningar per prenumeration.

Mer information om Azure RBAC-roller finns i [Azure RBAC-roller.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
