---
title: Flera användare får åtkomst nekad fel när du lägger till tillägg i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424176"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="bc39b-102">Flera användare får åtkomst nekad fel när du lägger till tillägg i Outlook</span><span class="sxs-lookup"><span data-stu-id="bc39b-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="bc39b-103">Du kan ange vilka administratörer i organisationen som har behörighet att installera och hantera tillägg för Outlook.</span><span class="sxs-lookup"><span data-stu-id="bc39b-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="bc39b-104">Du kan också ange vilka användare i organisationen som har behörighet att installera och hantera tillägg för eget bruk.</span><span class="sxs-lookup"><span data-stu-id="bc39b-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="bc39b-105">Mer information finns [i Ange vilka administratörer och användare som kan installera och hantera tillägg för Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="bc39b-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="bc39b-106">Om du vill kontrollera att du har tilldelat behörigheter för en användare ersätter du <Role Name> med namnet på rollen som ska verifieras och kör följande kommando i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="bc39b-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="bc39b-107">Get-ManagementRoleAssignment -Roll " <Role Name> " -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="bc39b-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="bc39b-108">I det här exemplet visas hur du verifierar vem du har tilldelat behörigheter för att installera tillägg från Office Store för organisationen.</span><span class="sxs-lookup"><span data-stu-id="bc39b-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="bc39b-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="bc39b-109">PowerShell</span></span>

<span data-ttu-id="bc39b-110">-Roll "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="bc39b-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="bc39b-111">I resultatet, Get-ManagementRoleAssignment, granska posterna i kolumnen Effektiva användare.</span><span class="sxs-lookup"><span data-stu-id="bc39b-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="bc39b-112">Detaljerad syntax- och parameterinformation finns i [Hämta-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="bc39b-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 