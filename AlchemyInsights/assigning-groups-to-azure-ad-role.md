---
title: Tilldela roller till Azure AD-rollen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885399"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="7c003-102">Tilldela roller till Azure AD-rollen</span><span class="sxs-lookup"><span data-stu-id="7c003-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="7c003-103">Så här tilldelar du en Azure AD-grupp med auktoritets källan i Azure AD till en Azure AD-roll:</span><span class="sxs-lookup"><span data-stu-id="7c003-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="7c003-104">Skapa en ny grupp – för att skapa en ny grupp:</span><span class="sxs-lookup"><span data-stu-id="7c003-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="7c003-105">a.</span><span class="sxs-lookup"><span data-stu-id="7c003-105">a.</span></span> <span data-ttu-id="7c003-106">Logga in på administrations centret för Azure AD med **Administratörs** behörighet för administratörer eller **Global administratör** .</span><span class="sxs-lookup"><span data-stu-id="7c003-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="7c003-107">b.</span><span class="sxs-lookup"><span data-stu-id="7c003-107">b.</span></span> <span data-ttu-id="7c003-108">Välj **> grupper i Azure Active Directory > alla grupper > ny grupp**.</span><span class="sxs-lookup"><span data-stu-id="7c003-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="7c003-109">c.</span><span class="sxs-lookup"><span data-stu-id="7c003-109">c.</span></span> <span data-ttu-id="7c003-110">Skapa gruppen.</span><span class="sxs-lookup"><span data-stu-id="7c003-110">Create the group.</span></span>

2. <span data-ttu-id="7c003-111">Tilldela rollen till gruppen antingen när grupp skapas eller efter att gruppen har skapats.</span><span class="sxs-lookup"><span data-stu-id="7c003-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="7c003-112">a.</span><span class="sxs-lookup"><span data-stu-id="7c003-112">a.</span></span> <span data-ttu-id="7c003-113">Om du vill tilldela en roll till gruppen när du skapar en grupp kan du byta till gruppen och skapa gruppen med växla mellan **Azure AD-rollerna** .</span><span class="sxs-lookup"><span data-stu-id="7c003-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="7c003-114">b.</span><span class="sxs-lookup"><span data-stu-id="7c003-114">b.</span></span> <span data-ttu-id="7c003-115">Om du vill tilldela en roll till gruppen efter att den har skapats navigerar du till fliken **tilldelade roller** för den nya gruppen och tilldelar rollen till gruppen.</span><span class="sxs-lookup"><span data-stu-id="7c003-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="7c003-116">**Hantera medlemskap för en grupp som är tilldelad Azure AD-rollen**</span><span class="sxs-lookup"><span data-stu-id="7c003-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="7c003-117">För att förhindra behörighets höjning, kan endast privilegierade roll administratörer och globala administratörer ändra medlemskap för en grupp som är tilldelad en roll.</span><span class="sxs-lookup"><span data-stu-id="7c003-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="7c003-118">De kan välja att tilldela en ägare för en sådan grupp och delegera uppgiften.</span><span class="sxs-lookup"><span data-stu-id="7c003-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="7c003-119">Mer information om hur du tilldelar moln grupper till Azure AD-roller finns i [tilldela en AD-roll till moln gruppen](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="7c003-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="7c003-120">Mer information om hur du felsöker roller tilldelade till moln grupper finns i [Felsöka roller som är tilldelade till moln grupper](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="7c003-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





