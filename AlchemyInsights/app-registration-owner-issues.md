---
title: Problem med appregistreringsägare
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405322"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="668f7-102">Problem med appregistreringsägare</span><span class="sxs-lookup"><span data-stu-id="668f7-102">App Registration Owner issues</span></span>

<span data-ttu-id="668f7-103">Här är de tillgängliga metoderna för att lägga till huvudnamn som ägare av appregistreringar:</span><span class="sxs-lookup"><span data-stu-id="668f7-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="668f7-104">Använda Azure AD PowerShell-modul –</span><span class="sxs-lookup"><span data-stu-id="668f7-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="668f7-105">Referens: [AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="668f7-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="668f7-106">Använda Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="668f7-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="668f7-107">Referens: [az ad-appägare](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="668f7-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="668f7-108">Använda MS Graph –</span><span class="sxs-lookup"><span data-stu-id="668f7-108">Using MS Graph -</span></span>

    <span data-ttu-id="668f7-109">Referens: [Lägg till ägare – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="668f7-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="668f7-110">Använda Azure AD-portalen – gå [till portal.azure.com](https://portal.azure.com/) > Azure Active Directory > appregistrering > Välj ditt program > ägare > Lägg till ägare</span><span class="sxs-lookup"><span data-stu-id="668f7-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="668f7-111">**Kan du inte visa ditt program i blad för appregistreringar trots att du är ägare till det programmet?**</span><span class="sxs-lookup"><span data-stu-id="668f7-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="668f7-112">Ägaren av en app är inte en administrativ roll.</span><span class="sxs-lookup"><span data-stu-id="668f7-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="668f7-113">Om inställningen Begränsa [åtkomst till Azure AD-administrationsportalen](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) är aktiverad kan bara administratören visa programmen på appregistreringsportalen.</span><span class="sxs-lookup"><span data-stu-id="668f7-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="668f7-114">För att en ägare ska kunna visa programmen inaktiverar du den här inställningen (Ange det som NEJ) eller tilldelar administratörsrollen till ägaren för bara det specifika programmet.</span><span class="sxs-lookup"><span data-stu-id="668f7-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="668f7-115">För detta behöver du dock en Azure AD Premium P2-licens och aktivera hantering [av privilegierad identitet.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="668f7-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
