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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583954"
---
# <a name="rbac-rules"></a>RBAC-regler

Om du får behörighets felet: 

- **Klienten med objekt-ID har inte behörighet att utföra en åtgärd via scope (kod: AuthorizationFailed)**: när du försöker skapa en resurs kontrollerar du att du är inloggad med en användare som har tilldelats en roll som har Skriv behörighet för resursen i det valda omfånget. Om du till exempel vill hantera virtuella datorer i en resurs grupp bör du ha rollen [virtuell dator deltagare](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) i resurs gruppen (eller det överordnade området). En lista över behörigheter för varje inbyggd roll finns i [fördefinierade roller för Azure-resurser](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Du har inte behörighet att skapa en supportbegäran**: när du försöker skapa eller uppdatera ett support ärende bör du kontrol lera att du är inloggad med en användare som har tilldelats en roll som har Microsoft. support/supportTickets/Skriv behörighet, till exempel [support deltagare](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- Det **går inte att skapa fler roll tilldelningar (kod: RoleAssignmentLimitExceeded)**: när du försöker tilldela en roll kan du försöka minska antalet roll tilldelningar genom att tilldela roller till grupper. Azure har stöd för upp till **2000** roll tilldelningar per prenumeration.

Mer information om Azure RBAC-roller finns i [Azure RBAC-roller](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
