---
title: Felsöka åtkomst nekad-meddelanden
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051443"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="cb1ac-102">Felsöka åtkomst nekad meddelanden i SharePoint/OneDrive administratörs Center</span><span class="sxs-lookup"><span data-stu-id="cb1ac-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="cb1ac-103">Om du får ett meddelande om nekad åtkomst när du försöker bläddra till en SharePoint/OneDrive administratörs Center, se till att du [tilldelar en licens till användaren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="cb1ac-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="cb1ac-104">Om användaren har en licens, bör du också se till att de har [tilldelats en administratörsroll](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som kan komma åt admin Centers.</span><span class="sxs-lookup"><span data-stu-id="cb1ac-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="cb1ac-105">Det här problemet kan också uppstå när en användare tas bort och återskapas med samma användarens huvudnamn (UPN).</span><span class="sxs-lookup"><span data-stu-id="cb1ac-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="cb1ac-106">Det nya kontot skapas med hjälp av ett annat PUID-värde (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="cb1ac-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="cb1ac-107">När användaren försöker komma åt en webbplatssamling eller deras OneDrive, har användaren en felaktig PUID.</span><span class="sxs-lookup"><span data-stu-id="cb1ac-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="cb1ac-108">Ett andra scenario innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="cb1ac-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="cb1ac-109">Om användarna redan har loggat in på SharePoint och sedan flyttas till en annan ORGANISATIONSENHET och synkroniseras med SharePoint, kan det här problemet uppstå.</span><span class="sxs-lookup"><span data-stu-id="cb1ac-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="cb1ac-110">Lös det här problemet bör du återställa det ursprungliga UPN-namnet med stegen i artikeln, [återställa en användare i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="cb1ac-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="cb1ac-111">Om ett OneDrive-eller SharePoint-administratörscenter inte är tillgängligt för flera användare som tidigare hade åtkomst kan det finnas ett tillfälligt tjänstproblem.</span><span class="sxs-lookup"><span data-stu-id="cb1ac-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="cb1ac-112">[Kontrollera den service Health instrumentpanelen](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="cb1ac-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


