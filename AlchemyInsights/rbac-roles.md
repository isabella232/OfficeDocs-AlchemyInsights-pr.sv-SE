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
# <a name="rbac-rules"></a><span data-ttu-id="2877a-102">RBAC-regler</span><span class="sxs-lookup"><span data-stu-id="2877a-102">RBAC rules</span></span>

<span data-ttu-id="2877a-103">Om du får behörighets felet:</span><span class="sxs-lookup"><span data-stu-id="2877a-103">If you get the permission error:</span></span> 

- <span data-ttu-id="2877a-104">**Klienten med objekt-ID har inte behörighet att utföra en åtgärd via scope (kod: AuthorizationFailed)**: när du försöker skapa en resurs kontrollerar du att du är inloggad med en användare som har tilldelats en roll som har Skriv behörighet för resursen i det valda omfånget.</span><span class="sxs-lookup"><span data-stu-id="2877a-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="2877a-105">Om du till exempel vill hantera virtuella datorer i en resurs grupp bör du ha rollen [virtuell dator deltagare](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) i resurs gruppen (eller det överordnade området).</span><span class="sxs-lookup"><span data-stu-id="2877a-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="2877a-106">En lista över behörigheter för varje inbyggd roll finns i [fördefinierade roller för Azure-resurser](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="2877a-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="2877a-107">**Du har inte behörighet att skapa en supportbegäran**: när du försöker skapa eller uppdatera ett support ärende bör du kontrol lera att du är inloggad med en användare som har tilldelats en roll som har Microsoft. support/supportTickets/Skriv behörighet, till exempel [support deltagare](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="2877a-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="2877a-108">Det **går inte att skapa fler roll tilldelningar (kod: RoleAssignmentLimitExceeded)**: när du försöker tilldela en roll kan du försöka minska antalet roll tilldelningar genom att tilldela roller till grupper.</span><span class="sxs-lookup"><span data-stu-id="2877a-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="2877a-109">Azure har stöd för upp till **2000** roll tilldelningar per prenumeration.</span><span class="sxs-lookup"><span data-stu-id="2877a-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="2877a-110">Mer information om Azure RBAC-roller finns i [Azure RBAC-roller](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="2877a-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
