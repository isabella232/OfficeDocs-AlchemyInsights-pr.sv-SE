---
title: 'Felsökning: åtkomst nekad meddelanden'
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f1a4803838b6511ef4fe7f03cafa4aa13b3c9734
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420718"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="03a39-102">Felsökning: åtkomst nekad meddelanden</span><span class="sxs-lookup"><span data-stu-id="03a39-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="03a39-103">Om någon har fått meddelandet ”åtkomst nekad” till en delad mapp kan administratören för webbplatssamlingen har aktiverat ”begränsad åtkomst användare behörighet låsning läge”.</span><span class="sxs-lookup"><span data-stu-id="03a39-103">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="03a39-104">Inaktivera det här:</span><span class="sxs-lookup"><span data-stu-id="03a39-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="03a39-105">Gå till webbplatsen, klicka på ikonen inställningar och klicka sedan på **Webbplatsinställningar**.</span><span class="sxs-lookup"><span data-stu-id="03a39-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="03a39-106">Klicka på **Webbplatssamlingens funktioner**under **Administration av webbplatssamling**.</span><span class="sxs-lookup"><span data-stu-id="03a39-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="03a39-107">Klicka på **Inaktivera**vid **begränsad åtkomst användarläge behörighet låsning**.</span><span class="sxs-lookup"><span data-stu-id="03a39-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="03a39-108">Ett meddelande om nekad åtkomst kan också uppstå för delade mappar om webbplatsen är en publiceringswebbplats.</span><span class="sxs-lookup"><span data-stu-id="03a39-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="03a39-109">Info, finns i [Åtkomst nekad när du ansluter till en delad mapp](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="03a39-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="03a39-110">Om en någon fick ett ”åtkomst nekad” visas när du försöker visa förfrågningar måste användaren som ska läggas till som administratör för en webbplatssamling eller en medlem av gruppen ägare för webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="03a39-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="03a39-111">Mer information finns i [Åtkomst nekad till listan åtkomstbegäranden](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="03a39-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="03a39-112">Om en användare har fått meddelandet ”åtkomst nekad” när de tas bort från Active Directory i lokaler och sedan lägga tillbaka, se [Åtkomst nekad när ett användarkonto är synkroniserad med Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="03a39-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

