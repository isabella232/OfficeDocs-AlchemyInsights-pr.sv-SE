---
title: Problem med att använda Administratörskonsolen Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555879"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="3f989-102">Problem med att använda Administratörskonsolen Intune</span><span class="sxs-lookup"><span data-stu-id="3f989-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="3f989-103">**"Åtkomst nekad" när du navigerar i Intune-administratörsportalen.**</span><span class="sxs-lookup"><span data-stu-id="3f989-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="3f989-104">Om du är medlem i en anpassad Intune-roll kontrollerar du att en EMS-licens (Intune eller Enterprise Mobility Suite) har tilldelats ditt konto.</span><span class="sxs-lookup"><span data-stu-id="3f989-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="3f989-105">Om du använder Configuration Manager för att hantera enheter kontrollerar du att du inte ingår i Intune-användarsamlingen för Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="3f989-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="3f989-106">Kontrollera att du har tilldelats lämpliga rollbaserade administrationskontroll (RBAC) behörigheter i Intune roller bladet.</span><span class="sxs-lookup"><span data-stu-id="3f989-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="3f989-107">Kontrollera att gruppen som används inte är en distributionslista.</span><span class="sxs-lookup"><span data-stu-id="3f989-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="3f989-108">Intune i Azure-portalen stöder endast användarkonton som tillhör Azure Active Directory-säkerhetsgrupper.</span><span class="sxs-lookup"><span data-stu-id="3f989-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="3f989-109">Granska dina grupper i Azure-portalen > **Intune**  >  **Groups**eller i Azure-portalen > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="3f989-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="3f989-110">**Användaren har för många behörigheter för tilldelad Intune-roll**</span><span class="sxs-lookup"><span data-stu-id="3f989-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="3f989-111">Råda användaren att gå till **Intune**  >  **Intune-roller**  >  **Mina behörigheter**  >  **Exportera** för granskning av beviljade behörigheter.</span><span class="sxs-lookup"><span data-stu-id="3f989-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="3f989-112">**Jag har lagt till en scopegrupp i en roll, men användare i den rollen ser fortfarande andra användare eller enheter.**</span><span class="sxs-lookup"><span data-stu-id="3f989-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="3f989-113">Scopegrupper filtrerar inte bort användare eller enheter.</span><span class="sxs-lookup"><span data-stu-id="3f989-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="3f989-114">Scopegrupper:</span><span class="sxs-lookup"><span data-stu-id="3f989-114">Scope groups:</span></span>

- <span data-ttu-id="3f989-115">Begränsa vem användare kan tilldela principer eller program till.</span><span class="sxs-lookup"><span data-stu-id="3f989-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="3f989-116">Tillåt endast specifika användare att köra fjärraktiviteter på enheter.</span><span class="sxs-lookup"><span data-stu-id="3f989-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="3f989-117">Mer information om scopegrupper finns i [Rollbaserad åtkomstkontroll (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="3f989-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="3f989-118">**Jag har lagt till en användare i en Intune-roll, men de har fortfarande full åtkomst till Intune-administratörskonsolen.**</span><span class="sxs-lookup"><span data-stu-id="3f989-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="3f989-119">Navigera till Intune > **användare** i Azure-portalen och kontrollera att användaren inte har tilldelats någon av följande roller i Azure-portalen:</span><span class="sxs-lookup"><span data-stu-id="3f989-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="3f989-120">Global administratör</span><span class="sxs-lookup"><span data-stu-id="3f989-120">Global administrator</span></span>
- <span data-ttu-id="3f989-121">Tjänstadministratör för Intune</span><span class="sxs-lookup"><span data-stu-id="3f989-121">Intune service administrator</span></span>
- <span data-ttu-id="3f989-122">SharePoint-administratör</span><span class="sxs-lookup"><span data-stu-id="3f989-122">SharePoint administrator</span></span>

<span data-ttu-id="3f989-123">Mer information finns i [Rollbaserad åtkomstkontroll (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="3f989-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="3f989-124">**Problem med åtkomst**</span><span class="sxs-lookup"><span data-stu-id="3f989-124">**Access Issues**</span></span>

<span data-ttu-id="3f989-125">Mer information finns [i Du kan inte logga in på Office 365, Azure eller Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="3f989-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>