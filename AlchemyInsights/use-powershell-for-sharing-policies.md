---
title: Använda Windows PowerShell för delningsprinciper och organisationsrelationer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709484"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="dbc67-102">Använda Windows PowerShell för delningsprinciper och organisationsrelationer</span><span class="sxs-lookup"><span data-stu-id="dbc67-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="dbc67-103">Information om organisationsrelationer finns i den detaljerade informationen om syntax och parametrar för: [Hämta federationsinformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [Ny organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Ange organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  och  [Ta bort organisationsrelation](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="dbc67-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="dbc67-104">För att skapa delningsprinciper, gå till [Ny delningsprincip](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="dbc67-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="dbc67-105">För att  [tillämpa en delningsprincip på en postlåda eller användare](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  måste du använda en kombination av  [Ange postlåda](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) och [Hämta postlåda](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) med den nya principen.</span><span class="sxs-lookup"><span data-stu-id="dbc67-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="dbc67-106">För att  [ändra, inaktivera eller ta bort en delningsprincip](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  måste du använda  [Ange delningsprincip](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) och [Ta bort delningsprincip](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="dbc67-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="dbc67-107">**Mer information för fullständig förståelse av det här avsnittet finns här:**</span><span class="sxs-lookup"><span data-stu-id="dbc67-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="dbc67-108">Delning i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="dbc67-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)