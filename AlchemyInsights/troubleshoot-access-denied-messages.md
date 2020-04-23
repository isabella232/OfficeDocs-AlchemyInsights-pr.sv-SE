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
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759818"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="daf3a-102">Felsöka nekade meddelanden om åtkomst</span><span class="sxs-lookup"><span data-stu-id="daf3a-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="daf3a-103">Om någon har fått meddelandet "Åtkomst nekad" till en delad mapp i SharePoint kan webbplatssamlingsadministratören ha aktiverat läget "Låsning av användarbehörighet med begränsad åtkomst".</span><span class="sxs-lookup"><span data-stu-id="daf3a-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="daf3a-104">Så här inaktiverar du detta:</span><span class="sxs-lookup"><span data-stu-id="daf3a-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="daf3a-105">Bläddra till webbplatsen, klicka på ikonen Inställningar och klicka sedan på **Webbplatsinställningar**.</span><span class="sxs-lookup"><span data-stu-id="daf3a-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="daf3a-106">Klicka på **Webbplatssamlingsfunktioner**under **Administration av webbplatssamling.**</span><span class="sxs-lookup"><span data-stu-id="daf3a-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="daf3a-107">Klicka på Inaktivera **bredvid låsningsläge för användarbehörighet**med begränsad åtkomst **.**</span><span class="sxs-lookup"><span data-stu-id="daf3a-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="daf3a-108">Ett meddelande om nekad åtkomst kan också visas för delade mappar om webbplatsen är en publiceringswebbplats.</span><span class="sxs-lookup"><span data-stu-id="daf3a-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="daf3a-109">Information finns i [Åtkomst nekad när du öppnar en delad mapp](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="daf3a-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="daf3a-110">Om en person fick meddelandet "Åtkomst nekad" när han eller hon försökte visa åtkomstbegäranden måste användaren läggas till som administratör för webbplatssamling eller medlem i gruppen Ägare för webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="daf3a-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="daf3a-111">Mer information finns i [listan Nekad åtkomstbegäran .](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="daf3a-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="daf3a-112">Om en användare har fått meddelandet "Åtkomst nekad" efter att de har tagits bort från Active Directory lokalt och sedan lagts till igen läser du [Nekad åtkomst när ett användarkonto synkroniseras med Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="daf3a-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

