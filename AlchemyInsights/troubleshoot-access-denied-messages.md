---
title: 'Felsökning: åtkomst nekad meddelanden'
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29491807"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="f1a0e-102">Felsökning: åtkomst nekad meddelanden</span><span class="sxs-lookup"><span data-stu-id="f1a0e-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="f1a0e-p101">Om någon har fått meddelandet ”åtkomst nekad” till en delad mapp kan administratören för webbplatssamlingen har aktiverat ”begränsad åtkomst användare behörighet låsning läge”. Inaktivera det här:</span><span class="sxs-lookup"><span data-stu-id="f1a0e-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="f1a0e-105">Gå till webbplatsen, klicka på ikonen inställningar och klicka sedan på **Webbplatsinställningar**.</span><span class="sxs-lookup"><span data-stu-id="f1a0e-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="f1a0e-106">Klicka på **Webbplatssamlingens funktioner**under **Administration av webbplatssamling**.</span><span class="sxs-lookup"><span data-stu-id="f1a0e-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="f1a0e-107">Klicka på **Inaktivera**vid **begränsad åtkomst användarläge behörighet låsning**.</span><span class="sxs-lookup"><span data-stu-id="f1a0e-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="f1a0e-p102">Ett meddelande om nekad åtkomst kan också uppstå för delade mappar om webbplatsen är en publiceringswebbplats. Info, finns i [Åtkomst nekad när du ansluter till en delad mapp](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="f1a0e-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="f1a0e-p103">Om en någon fick ett ”åtkomst nekad” visas när du försöker visa förfrågningar måste användaren som ska läggas till som administratör för en webbplatssamling eller en medlem av gruppen ägare för webbplatsen. Mer information finns i [Åtkomst nekad till listan åtkomstbegäranden](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="f1a0e-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="f1a0e-112">Om en användare har fått meddelandet ”åtkomst nekad” när de tas bort från Active Directory i lokaler och sedan lägga tillbaka, se [Åtkomst nekad när ett användarkonto är synkroniserad med Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="f1a0e-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

