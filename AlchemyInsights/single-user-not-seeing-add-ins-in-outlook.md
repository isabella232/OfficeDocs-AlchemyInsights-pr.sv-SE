---
title: En användare ser inte tillägg i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198221"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="54b51-102">En användare ser inte tillägg i Outlook</span><span class="sxs-lookup"><span data-stu-id="54b51-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="54b51-103">Användaren kan vara en del av en roll som inte har rätt AppsForOfficeEnabled-parameter.</span><span class="sxs-lookup"><span data-stu-id="54b51-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="54b51-104">Kör den här cmdleten för att ta reda på om rätt roll är associerad med användaren:</span><span class="sxs-lookup"><span data-stu-id="54b51-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="54b51-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegera $false | Format-tabell -Auto roll,RollAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="54b51-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="54b51-106">Mer information finns [i Ange vilka administratörer och användare som kan installera och hantera tillägg för Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="54b51-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
