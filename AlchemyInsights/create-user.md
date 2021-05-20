---
title: Skapa användare
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569765"
---
# <a name="create-user"></a><span data-ttu-id="f228b-102">Skapa användare</span><span class="sxs-lookup"><span data-stu-id="f228b-102">Create user</span></span>

<span data-ttu-id="f228b-103">**MEDDELANDE:**</span><span class="sxs-lookup"><span data-stu-id="f228b-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="f228b-104">[Utfasning av WebView-inloggningssupport från Google från och med den 4 januari 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="f228b-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="f228b-105">Testa om dina appar kan påverkas av att [följa Googles anvisningar](https://go.microsoft.com/fwlink/?linkid=2157323) om kompatibilitetstestning.</span><span class="sxs-lookup"><span data-stu-id="f228b-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="f228b-106">Kontrollera att du använder systemets webbvy eller systemwebbläsare när du loggar in dina användare med Google-konsumentkonton.</span><span class="sxs-lookup"><span data-stu-id="f228b-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="f228b-107">Mer information finns i [Problem med att logga in på program med bara Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span><span class="sxs-lookup"><span data-stu-id="f228b-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="f228b-108">**Jag kan inte skapa en ny användare i min Azure AD-katalog**</span><span class="sxs-lookup"><span data-stu-id="f228b-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="f228b-109">Se till att du har behörighet att skapa en ny standardanvändare.</span><span class="sxs-lookup"><span data-stu-id="f228b-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="f228b-110">Endast rollen global administratör eller användaradministratör i Azure Active Directory (AD) kan skapa en ny standardanvändare.</span><span class="sxs-lookup"><span data-stu-id="f228b-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="f228b-111">Om du inte har någon av dessa roller kan du be en administratör att lägga till dig i en av rollerna eller att skapa det nya användarkontot åt dig.</span><span class="sxs-lookup"><span data-stu-id="f228b-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="f228b-112">Kontrollera att användarnamnet finns i en domän som har verifierats i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f228b-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="f228b-113">Om du inte har några verifierade anpassade domännamn i azure AD kan du använda din initiala Azure AD-domän, som slutar med \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="f228b-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="f228b-114">Kontrollera att användarnamnet finns i en domän som inte är federerad till Azure AD från din lokala AD.</span><span class="sxs-lookup"><span data-stu-id="f228b-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="f228b-115">Användare kan inte läggas till i molnet med domännamn som är externa från lokalt.</span><span class="sxs-lookup"><span data-stu-id="f228b-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="f228b-116">Kontrollera att ingen annan användare eller kontakt redan har det användarnamn som du vill tilldela den nya användaren.</span><span class="sxs-lookup"><span data-stu-id="f228b-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="f228b-117">Användarnamn måste vara unika för alla Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f228b-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="f228b-118">Se [Azure AD-roller och -administratörer](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) för Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f228b-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="f228b-119">Se [domännamnen för](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f228b-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="f228b-120">Granska [granskningsloggar](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) om du vill se mer detaljerad information om en nyligen skapad eller borttagna användare, till exempel vem som utförde åtgärden och när.</span><span class="sxs-lookup"><span data-stu-id="f228b-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="f228b-121">Mer information om hur du lägger till nya användare finns [i Använda Azure Portal för att skapa en ny användare i azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="f228b-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="f228b-122">[Azure AD-administratörsroller:](/azure/active-directory/active-directory-assign-admin-roles)Administratörsrollbehörigheter i Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f228b-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="f228b-123">Du kan också [använda Azure AD PowerShell för att skapa en ny användare.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="f228b-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
