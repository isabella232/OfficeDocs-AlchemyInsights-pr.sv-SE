---
title: Gruppsynkronisering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256916"
---
# <a name="group-sync"></a><span data-ttu-id="b3240-102">Gruppsynkronisering</span><span class="sxs-lookup"><span data-stu-id="b3240-102">Group sync</span></span>

<span data-ttu-id="b3240-103">Den här artikeln innehåller vägledning om gruppsynkronisering.</span><span class="sxs-lookup"><span data-stu-id="b3240-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="b3240-104">Om en global administratör eller gruppägare inte kan ändra gruppegenskaper eller lägga till medlemmar eller tilldela ägare i Azure-portalen ser du till att källan för gruppen är Azure Active Directory (Azure AD) för den globala administratören eller gruppägaren för att ändra gruppen.</span><span class="sxs-lookup"><span data-stu-id="b3240-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="b3240-105">Innan du försöker ta bort en synkroniserad grupp i Azure AD bör du kontrollera att du [har tagit bort alla tilldelade licenser för](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) att undvika fel.</span><span class="sxs-lookup"><span data-stu-id="b3240-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="b3240-106">Mer information om hur du synkroniserar användare, grupper och kontakter finns i [Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)och hur du följer Synkronisering av en lokal grupp till Azure med hjälp av [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) för att synkronisera lokala grupper med AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b3240-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="b3240-107">Följ de här [guiderna för felsökning av fel under synkroniseringen](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) för att felsöka vanliga fel under synkroniseringen.</span><span class="sxs-lookup"><span data-stu-id="b3240-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

