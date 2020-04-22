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
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758537"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="8ba51-102">Felsöka nekade meddelanden i Administrationscenter för Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="8ba51-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="8ba51-103">Om du får ett meddelande om nekad åtkomst när du försöker bläddra till ett Administrationscenter för Sharepoint/OneDrive kontrollerar du att du [tilldelar användaren en licens](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="8ba51-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="8ba51-104">Om användaren har en licens bör du också se till att de [tilldelas en administratörsroll](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som kan komma åt administratörscentren.</span><span class="sxs-lookup"><span data-stu-id="8ba51-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="8ba51-105">Det här problemet kan också uppstå när en användare tas bort och återskapas med samma användarnamn (UPN).</span><span class="sxs-lookup"><span data-stu-id="8ba51-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="8ba51-106">Det nya kontot skapas med hjälp av ett annat PUID-värde (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="8ba51-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="8ba51-107">När användaren försöker komma åt en webbplatssamling eller sin OneDrive har användaren ett felaktigt PUID.</span><span class="sxs-lookup"><span data-stu-id="8ba51-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="8ba51-108">Ett andra scenario innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="8ba51-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="8ba51-109">Om användare redan har loggat in på SharePoint och sedan flyttas till en annan organisationsenhet och synkroniseras med SharePoint, kan det här problemet uppstå.</span><span class="sxs-lookup"><span data-stu-id="8ba51-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="8ba51-110">LÃ¶s problemet genom att återställa det ursprungliga UPN med stegen i artikeln, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="8ba51-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="8ba51-111">Om ett OneDrive- eller SharePoint-administrationscenter inte är tillgängligt för flera användare som tidigare hade åtkomst kan det bero på ett tillfälligt serviceproblem.</span><span class="sxs-lookup"><span data-stu-id="8ba51-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="8ba51-112">[Kontrollera instrumentpanelen för tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8ba51-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


