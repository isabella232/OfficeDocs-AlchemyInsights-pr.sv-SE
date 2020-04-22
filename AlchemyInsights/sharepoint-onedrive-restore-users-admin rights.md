---
title: Felsöka åtkomst nekade meddelanden till OneDrive för företag-webbplatser
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692819"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="d446d-102">Felsöka åtkomst nekade meddelanden till OneDrive för företag-webbplatser</span><span class="sxs-lookup"><span data-stu-id="d446d-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="d446d-103">Det här problemet uppstår oftast när en användare tas bort och återskapas med samma användarnamn (UPN).</span><span class="sxs-lookup"><span data-stu-id="d446d-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="d446d-104">Det nya kontot skapas med hjälp av ett annat PUID-värde (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="d446d-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="d446d-105">När användaren försöker komma åt en webbplatssamling eller sin OneDrive har användaren ett felaktigt PUID.</span><span class="sxs-lookup"><span data-stu-id="d446d-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="d446d-106">Ett andra scenario innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="d446d-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="d446d-107">Om användare redan har loggat in på SharePoint och sedan flyttas till en annan organisationsenhet och synkroniseras med SharePoint, kan det här problemet uppstå.</span><span class="sxs-lookup"><span data-stu-id="d446d-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="d446d-108">LÃ¶s problemet genom att återställa det ursprungliga UPN med stegen i artikeln, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="d446d-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="d446d-109">Om du inte kan återställa den ursprungliga användaren bör du ta bort den gamla användaren från OneDrive-webbplatsen med hjälp av dessa [steg, Ta bort en användare från listan användarinformation]().</span><span class="sxs-lookup"><span data-stu-id="d446d-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="d446d-110">När detta är gjort kan du kontrollera att användaren har administratörsrättigheter till OneDrive-webbplatsen genom att följa stegen [i Lägg till administratör för en användares OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="d446d-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="d446d-111">Mer information om behörighetsnivåer finns i artikeln [Förstå behörighetsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="d446d-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
