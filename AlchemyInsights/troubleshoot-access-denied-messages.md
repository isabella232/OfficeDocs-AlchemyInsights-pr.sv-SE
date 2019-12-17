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
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050723"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="5eb1a-102">Felsöka åtkomst nekad-meddelanden</span><span class="sxs-lookup"><span data-stu-id="5eb1a-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="5eb1a-103">Om någon har fått meddelandet "åtkomst nekad" till en delad mapp i SharePoint, kan administratören för webbplatssamlingen ha aktiverat läget "begränsad åtkomst till användarbehörighet".</span><span class="sxs-lookup"><span data-stu-id="5eb1a-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="5eb1a-104">Så här stänger du av:</span><span class="sxs-lookup"><span data-stu-id="5eb1a-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="5eb1a-105">Bläddra till webbplatsen, klicka på ikonen Inställningar och klicka sedan på **Webbplatsinställningar**.</span><span class="sxs-lookup"><span data-stu-id="5eb1a-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="5eb1a-106">Klicka på **Webbplatssamlingens funktioner**under **Administration av webbplatssamling**.</span><span class="sxs-lookup"><span data-stu-id="5eb1a-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="5eb1a-107">Bredvid **begränsad åtkomst användarbehörighet låsning läge**, klickar du på **inaktivera**.</span><span class="sxs-lookup"><span data-stu-id="5eb1a-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="5eb1a-108">Ett meddelande om nekad åtkomst kan också uppstå för delade mappar om webbplatsen är en publiceringswebbplats.</span><span class="sxs-lookup"><span data-stu-id="5eb1a-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="5eb1a-109">Mer information finns i [åtkomst nekad vid åtkomst till en delad mapp](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="5eb1a-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="5eb1a-110">Om en person har fått meddelandet "åtkomst nekad" när du försöker visa åtkomstbegäranden måste användaren läggas till som en webbplatssamlingsadministratör eller medlem i gruppen ägare för webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="5eb1a-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="5eb1a-111">Mer information finns i [åtkomst nekad till listan åtkomstbegäranden](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="5eb1a-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="5eb1a-112">Om en användare har fått meddelandet "åtkomst nekad" efter att de har tagits bort från Active Directory lokalt och sedan lagts till igen, se [åtkomst nekad när ett användarkonto har synkroniserats till Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="5eb1a-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

