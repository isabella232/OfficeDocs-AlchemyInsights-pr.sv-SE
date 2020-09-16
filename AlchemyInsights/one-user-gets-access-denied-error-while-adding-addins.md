---
title: En användare får åtkomst nekat-fel när tillägg läggs till i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 355f37386e0a498185e195c1d715386785d0b54b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673299"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="f031b-102">En användare får åtkomst nekat-fel när tillägg läggs till i Outlook</span><span class="sxs-lookup"><span data-stu-id="f031b-102">One user gets Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="f031b-103">User PowerShell för att hitta behörigheter:</span><span class="sxs-lookup"><span data-stu-id="f031b-103">User PowerShell To find permissions:</span></span>

<span data-ttu-id="f031b-104">Get-ManagementRoleAssignment-RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -delegera $false | Format-automatisk roll för tabeller, RoleAssigneeName, RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="f031b-104">Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>