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
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690801"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="14b23-102">Felsöka åtkomst nekade meddelanden</span><span class="sxs-lookup"><span data-stu-id="14b23-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="14b23-103">Om någon har fått meddelandet "åtkomst nekad" till en delad mapp i SharePoint kan administratören för webbplats samlingen ha aktiverat lås läge för användare med begränsad åtkomst.</span><span class="sxs-lookup"><span data-stu-id="14b23-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="14b23-104">Så här inaktiverar du det:</span><span class="sxs-lookup"><span data-stu-id="14b23-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="14b23-105">Bläddra till webbplatsen, klicka på ikonen Inställningar och sedan på **webbplats inställningar**.</span><span class="sxs-lookup"><span data-stu-id="14b23-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="14b23-106">Klicka på **webbplats samlingens funktioner**under **Administration av webbplats samling**.</span><span class="sxs-lookup"><span data-stu-id="14b23-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="14b23-107">Bredvid **nedlåst behörighets läge för användare med begränsad åtkomst**klickar du på **inaktivera**.</span><span class="sxs-lookup"><span data-stu-id="14b23-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="14b23-108">Ett meddelande om nekad åtkomst kan också förekomma för delade mappar om webbplatsen är en publicerings webbplats.</span><span class="sxs-lookup"><span data-stu-id="14b23-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="14b23-109">Mer information finns i [åtkomst nekad när du öppnar en delad mapp](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="14b23-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="14b23-110">Om en person fick meddelandet "åtkomst nekad" när du försöker visa åtkomst begär Anden måste användaren läggas till som administratör för en webbplats samling eller medlem i gruppen ägare för webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="14b23-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="14b23-111">Mer information finns i [åtkomst nekad till listan med åtkomst förfrågningar](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="14b23-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="14b23-112">Om en användare har fått meddelandet "åtkomst nekad" efter att de tagits bort från Active Directory lokalt och sedan återlagts, kan [du läsa åtkomst nekad när ett användar konto synkroniseras till Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="14b23-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

