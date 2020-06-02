---
title: Felsöka nekade meddelanden om åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505397"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="397fa-102">Felsöka nekade meddelanden i Administrationscenter för Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="397fa-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="397fa-103">Om du får ett meddelande om nekad åtkomst när du försöker bläddra till ett Administrationscenter för Sharepoint/OneDrive kontrollerar du att du [tilldelar användaren en licens](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="397fa-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="397fa-104">Om användaren har en licens bör du också se till att de [tilldelas en administratörsroll](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som kan komma åt administratörscentren.</span><span class="sxs-lookup"><span data-stu-id="397fa-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="397fa-105">Det här problemet kan också uppstå när en användare tas bort och återskapas med samma användarnamn (UPN).</span><span class="sxs-lookup"><span data-stu-id="397fa-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="397fa-106">Det nya kontot skapas med hjälp av ett annat PUID-värde (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="397fa-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="397fa-107">När användaren försöker komma åt en webbplatssamling eller sin OneDrive har användaren ett felaktigt PUID.</span><span class="sxs-lookup"><span data-stu-id="397fa-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="397fa-108">Ett andra scenario innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="397fa-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="397fa-109">Om användare redan har loggat in på SharePoint och sedan flyttas till en annan organisationsenhet och synkroniseras med SharePoint, kan det här problemet uppstå.</span><span class="sxs-lookup"><span data-stu-id="397fa-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="397fa-110">LÃ¶s problemet genom att återställa det ursprungliga UPN med stegen i artikeln, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="397fa-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="397fa-111">Om ett OneDrive- eller SharePoint-administrationscenter inte är tillgängligt för flera användare som tidigare hade åtkomst kan det bero på ett tillfälligt serviceproblem.</span><span class="sxs-lookup"><span data-stu-id="397fa-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="397fa-112">[Kontrollera instrumentpanelen för tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="397fa-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


