---
title: Det går inte att ändra Användarnamn
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440297"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="3c035-102">Det går inte att ändra Användarnamn</span><span class="sxs-lookup"><span data-stu-id="3c035-102">Unable to change UserName</span></span>

<span data-ttu-id="3c035-103">I vissa fall sprids inte UPN-ändringar (UserPrincipalName) till molnet.</span><span class="sxs-lookup"><span data-stu-id="3c035-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="3c035-104">Valideringsfel kan visas i Office 365-portalen eller inte ändra användarnamnet eller e-postadressen.</span><span class="sxs-lookup"><span data-stu-id="3c035-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="3c035-105">LÃ¶s problemet genom att ange UserPrincipalName manuellt med det här PowerShell-kommandot.</span><span class="sxs-lookup"><span data-stu-id="3c035-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="3c035-106">**Exempel: Byta namn på en användare**</span><span class="sxs-lookup"><span data-stu-id="3c035-106">**Example: Rename a user**</span></span>

<span data-ttu-id="3c035-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="3c035-107">PowerShellCopy</span></span>

<span data-ttu-id="3c035-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="3c035-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="3c035-109">Det här kommandot byter namn på davidc@contoso.com till davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="3c035-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="3c035-110">Mer information finns i [Ange-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="3c035-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>