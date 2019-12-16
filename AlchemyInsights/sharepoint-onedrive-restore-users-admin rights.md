---
title: Felsöka åtkomst nekad meddelanden till OneDrive för Business-webbplatser
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051623"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="58256-102">Felsöka åtkomst nekad meddelanden till OneDrive för Business-webbplatser</span><span class="sxs-lookup"><span data-stu-id="58256-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="58256-103">Det här problemet uppstår oftast när en användare tas bort och återskapas med samma användarens huvudnamn (UPN).</span><span class="sxs-lookup"><span data-stu-id="58256-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="58256-104">Det nya kontot skapas med hjälp av ett annat PUID-värde (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="58256-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="58256-105">När användaren försöker komma åt en webbplatssamling eller deras OneDrive, har användaren en felaktig PUID.</span><span class="sxs-lookup"><span data-stu-id="58256-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="58256-106">Ett andra scenario innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="58256-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="58256-107">Om användarna redan har loggat in på SharePoint och sedan flyttas till en annan ORGANISATIONSENHET och synkroniseras med SharePoint, kan det här problemet uppstå.</span><span class="sxs-lookup"><span data-stu-id="58256-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="58256-108">Lös det här problemet bör du återställa den ursprungliga UPN med stegen i artikeln, [återställa en användare i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="58256-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="58256-109">Om du inte kan återställa den ursprungliga användaren bör du ta bort den gamla användaren från OneDrive-webbplatsen med hjälp av dessa steg, [ta bort en användare från listan användarinformation]().</span><span class="sxs-lookup"><span data-stu-id="58256-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="58256-110">När detta är gjort kan du kontrollera att användaren har administratörsrättigheter till webbplatsen för OneDrive genom att följa stegen för att [lägga till admin för en användares OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="58256-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="58256-111">Mer information om behörighetsnivåer finns i artikeln [förstå behörighetsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="58256-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
