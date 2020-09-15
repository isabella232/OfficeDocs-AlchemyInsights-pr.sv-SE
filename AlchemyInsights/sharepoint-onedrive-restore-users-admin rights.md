---
title: Felsöka åtkomst nekade till OneDrive för företag-webbplatser
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670634"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="8dc82-102">Felsöka åtkomst nekade till OneDrive för företag-webbplatser</span><span class="sxs-lookup"><span data-stu-id="8dc82-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="8dc82-103">Det här problemet uppstår ofta när en användare tas bort och återskapas med samma huvud namn (UPN).</span><span class="sxs-lookup"><span data-stu-id="8dc82-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="8dc82-104">Det nya kontot skapas med ett annat PUID-värde (unikt ID).</span><span class="sxs-lookup"><span data-stu-id="8dc82-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="8dc82-105">När användaren försöker komma åt en webbplats samling eller deras OneDrive har användaren felaktigt PUID.</span><span class="sxs-lookup"><span data-stu-id="8dc82-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="8dc82-106">Ett andra scenario inkluderar profilsynkronisering med en Active Directory-organisationsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="8dc82-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="8dc82-107">Om användare redan har loggat in i SharePoint och sedan flyttas till en annan ORGANISATIONSENHET och synkroniseras med SharePoint, kan de uppleva det här problemet.</span><span class="sxs-lookup"><span data-stu-id="8dc82-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="8dc82-108">Lös problemet genom att återställa den ursprungliga UPN-filen enligt anvisningarna i artikeln [Återställ en användare i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="8dc82-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="8dc82-109">Om du inte kan återställa den ursprungliga användaren bör du ta bort den gamla användaren från OneDrive-webbplatsen genom att följa de här stegen och [ta bort en användare från listan med användar information]().</span><span class="sxs-lookup"><span data-stu-id="8dc82-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="8dc82-110">När det är klart kan du kontrol lera att användaren har administratörs behörighet för OneDrive-webbplatsen genom att följa anvisningarna för att [lägga till administratörens för en användares OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="8dc82-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="8dc82-111">Mer information om behörighets nivåer finns i artikeln [förstå behörighets nivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="8dc82-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
