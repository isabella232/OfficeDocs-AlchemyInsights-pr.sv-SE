---
title: Felsöka ägar problem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901276"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="a84a0-102">Felsöka ägar problem</span><span class="sxs-lookup"><span data-stu-id="a84a0-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="a84a0-103">Så här felsöker du problem med ägaren:</span><span class="sxs-lookup"><span data-stu-id="a84a0-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="a84a0-104">[Lägga till eller ändra Azure-abonnemang administratörer](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure AD-grupper ägs och hanteras av grupp ägare.</span><span class="sxs-lookup"><span data-stu-id="a84a0-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="a84a0-105">Grupp ägare kan vara användare eller tjänstens huvud män och kan hantera gruppen, inklusive medlemskap.</span><span class="sxs-lookup"><span data-stu-id="a84a0-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="a84a0-106">Endast befintliga grupp ägare eller grupp-hanterar administratörer kan tilldela grupp ägare.</span><span class="sxs-lookup"><span data-stu-id="a84a0-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="a84a0-107">Grupp ägare måste inte vara medlemmar i gruppen.</span><span class="sxs-lookup"><span data-stu-id="a84a0-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="a84a0-108">[Lägga till eller ändra Azure-prenumerations administratörer](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): i den här artikeln beskrivs hur du lägger till eller ändrar administratörs rollen för en användare med Azure RBAC i prenumerations omfattningen.</span><span class="sxs-lookup"><span data-stu-id="a84a0-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="a84a0-109">Använd PowerShell för att lägga till en grupp ägare eller en program ägare.</span><span class="sxs-lookup"><span data-stu-id="a84a0-109">Use PowerShell to add a group owner or an application owner.</span></span>
