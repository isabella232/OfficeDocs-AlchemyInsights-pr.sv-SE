---
title: Roll för privilegie rad identitet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089150"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="9e454-102">Rollen som privilegierad identitets hantering (PIM)</span><span class="sxs-lookup"><span data-stu-id="9e454-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="9e454-103">**Behörigheter beviljas inte efter aktivering av en roll**</span><span class="sxs-lookup"><span data-stu-id="9e454-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="9e454-104">När du aktiverar en roll i Azure AD Report Management (PIM) kan aktivering inte omedelbart spridas till alla portaler som kräver den privilegierade rollen.</span><span class="sxs-lookup"><span data-stu-id="9e454-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="9e454-105">Ibland, även om ändringen sprids kan det hända att ändringarna inte börjar gälla omedelbart.</span><span class="sxs-lookup"><span data-stu-id="9e454-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="9e454-106">Om aktiveringen är försenad gör du följande:</span><span class="sxs-lookup"><span data-stu-id="9e454-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="9e454-107">Logga ut från Azure-portalen och logga sedan in igen.</span><span class="sxs-lookup"><span data-stu-id="9e454-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="9e454-108">När du aktiverar en Azure AD-roll eller en Azure-adressresurs visas stegen i din aktivering.</span><span class="sxs-lookup"><span data-stu-id="9e454-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="9e454-109">När alla stadier är klara visas en "Logga ut"-länk.</span><span class="sxs-lookup"><span data-stu-id="9e454-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="9e454-110">Du kan använda den här länken för att logga ut. Detta löser de flesta fall för aktiverings fördröjning.</span><span class="sxs-lookup"><span data-stu-id="9e454-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="9e454-111">I PIM kontrollerar du att du är angiven som medlem i rollen.</span><span class="sxs-lookup"><span data-stu-id="9e454-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="9e454-112">Om du aktiverar rollen som Exchange-administratör kontrollerar du att du loggar ut och loggar in igen.</span><span class="sxs-lookup"><span data-stu-id="9e454-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="9e454-113">Om problemet kvarstår öppnar du ett support ärende och får ett problem.</span><span class="sxs-lookup"><span data-stu-id="9e454-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="9e454-114">Om du använder rollen som Exchange-administratör för att få åtkomst till säkerhets-och efterlevnadsprinciper finns i nästa steg.</span><span class="sxs-lookup"><span data-stu-id="9e454-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="9e454-115">Om du aktiverar en roll för att få åtkomst till säkerhets-och efterföljandekrav eller om du aktiverar SharePoint-administratörskonsolen kommer det att inträffa en viss aktiverings fördröjning från några minuter upp till några timmar.</span><span class="sxs-lookup"><span data-stu-id="9e454-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="9e454-116">Detta är ett känt problem och vi samarbetar aktivt med dessa team för att lösa problemet så snart som möjligt.</span><span class="sxs-lookup"><span data-stu-id="9e454-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="9e454-117">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="9e454-117">For more information, see:</span></span>

- [<span data-ttu-id="9e454-118">Aktivera mina Azure AD-roller i PIM</span><span class="sxs-lookup"><span data-stu-id="9e454-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="9e454-119">Aktivera mina Azure Resource-roller i PIM</span><span class="sxs-lookup"><span data-stu-id="9e454-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="9e454-120">**Behörigheter tas inte bort när du har inaktiverat en roll eller om roll aktiveringen upphör**</span><span class="sxs-lookup"><span data-stu-id="9e454-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="9e454-121">När du inaktiverar en roll i Azure AD-privilegierad identitets hantering eller när en aktiverings period för en roll upphör kan det bero på att du har fortsatt åtkomst.</span><span class="sxs-lookup"><span data-stu-id="9e454-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="9e454-122">Om inaktive ringen är fördröjd gör du följande:</span><span class="sxs-lookup"><span data-stu-id="9e454-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="9e454-123">Om du inaktiverar rollen som Exchange-administratör eller om roll aktiverings perioden går ut, och du får en avsevärd fördröjning innan behörigheterna tas bort, öppnar du ett support ärende och ber din support ingenjör att hjälpa dig att arkivera en biljett med PAM-teamet i Office om det här problemet.</span><span class="sxs-lookup"><span data-stu-id="9e454-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="9e454-124">Om aktiverings perioden har gått ut men du fortfarande har webbläsarsessionen öppen stänger du webbläsaren.</span><span class="sxs-lookup"><span data-stu-id="9e454-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="9e454-125">Du kan fortsätta att använda rollen tills du stänger den sessionen.</span><span class="sxs-lookup"><span data-stu-id="9e454-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="9e454-126">Detta är ett känt problem och vi tittar på en möjlig åtgärd för att aktivt återkalla varje session när aktiveringen har upphört att gälla.</span><span class="sxs-lookup"><span data-stu-id="9e454-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="9e454-127">Om din fördröjning är annorlunda än de här två fallen måste du öppna ett support ärende.</span><span class="sxs-lookup"><span data-stu-id="9e454-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
