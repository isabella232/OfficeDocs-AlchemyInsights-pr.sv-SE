---
title: Felsöka åtkomst nekad meddelanden till OneDrive för Business-platser
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354815"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="acefc-102">Felsöka åtkomst nekad meddelanden till OneDrive för Business-platser</span><span class="sxs-lookup"><span data-stu-id="acefc-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="acefc-103">Det här problemet uppstår oftast när en användare tas bort och återskapas med samma användarhuvudnamn (UPN).</span><span class="sxs-lookup"><span data-stu-id="acefc-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="acefc-104">Det nya kontot har skapats med ett annat värde PUID (Passport unika ID).</span><span class="sxs-lookup"><span data-stu-id="acefc-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="acefc-105">När användaren försöker komma åt en webbplatssamling eller deras OneDrive, har användaren en felaktig PUID.</span><span class="sxs-lookup"><span data-stu-id="acefc-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="acefc-106">Andra scenariot innebär katalogsynkronisering med en Active Directory-organisationsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="acefc-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="acefc-107">Om användare har redan inloggad i SharePoint, och har flyttats till en annan Organisationsenhet och resynced med SharePoint, kan problemet uppstå.</span><span class="sxs-lookup"><span data-stu-id="acefc-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="acefc-108">Lös det här problemet bör du återställa den ursprungliga UPN med åtgärderna i artikeln[återställa en användare i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="acefc-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="acefc-109">När detta är gjort kan verifiera du användaren har admin rättigheter till OneDrive-webbplatsen genom att följa instruktionerna för att [lägga till admin tillhör en användare OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="acefc-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="acefc-110">Mer information om behörighetsnivåer finns i artikeln [Förstå behörighetsnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="acefc-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
