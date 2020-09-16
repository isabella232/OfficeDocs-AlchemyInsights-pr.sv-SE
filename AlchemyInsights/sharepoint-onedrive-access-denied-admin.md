---
title: Felsöka åtkomst nekade meddelanden
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767681"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="284ab-102">Felsöka åtkomst nekade meddelanden i administrations centret för SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="284ab-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="284ab-103">Om du får ett meddelande om nekad åtkomst när du försöker bläddra till ett administrations Center för SharePoint/OneDrive måste du [tilldela en licens till användaren](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="284ab-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="284ab-104">Om användaren har en licens bör du också kontrol lera att de [tilldelats en administratörs roll](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som har åtkomst till administrations centret.</span><span class="sxs-lookup"><span data-stu-id="284ab-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="284ab-105">Det här problemet kan även uppstå när en användare tas bort och återskapas med samma huvud namn (UPN).</span><span class="sxs-lookup"><span data-stu-id="284ab-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="284ab-106">Det nya kontot skapas med ett annat PUID-värde (unikt ID).</span><span class="sxs-lookup"><span data-stu-id="284ab-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="284ab-107">När användaren försöker komma åt en webbplats samling eller deras OneDrive har användaren felaktigt PUID.</span><span class="sxs-lookup"><span data-stu-id="284ab-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="284ab-108">Ett andra scenario inkluderar profilsynkronisering med en Active Directory-organisationsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="284ab-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="284ab-109">Om användare redan har loggat in i SharePoint och sedan flyttas till en annan ORGANISATIONSENHET och synkroniseras med SharePoint, kan de uppleva det här problemet.</span><span class="sxs-lookup"><span data-stu-id="284ab-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="284ab-110">Lös problemet genom att återställa den ursprungliga UPN-informationen enligt anvisningarna i artikeln [återställa en användare i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="284ab-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="284ab-111">OBS! om ett OneDrive-eller SharePoint-administrationsobjekt inte är tillgängligt för flera användare som tidigare hade åtkomst kan det finnas ett tillfälligt tjänst problem.</span><span class="sxs-lookup"><span data-stu-id="284ab-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="284ab-112">[Kontrol lera instrument panelen för tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="284ab-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


