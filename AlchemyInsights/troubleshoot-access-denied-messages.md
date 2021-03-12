---
title: Felsöka meddelanden om nekad åtkomst
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704912"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="7626b-102">Felsöka meddelanden om nekad åtkomst</span><span class="sxs-lookup"><span data-stu-id="7626b-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="7626b-103">Om någon fick meddelandet "Åtkomst nekad" till en delad mapp i SharePoint kan webbplatssamlingsadministratören ha aktiverat nedlåst behörighetsläge för användare med begränsad åtkomst.</span><span class="sxs-lookup"><span data-stu-id="7626b-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="7626b-104">Så här inaktiverar du det här:</span><span class="sxs-lookup"><span data-stu-id="7626b-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="7626b-105">Bläddra till webbplatsen, klicka på ikonen Inställningar och klicka sedan på **Webbplatsinställningar.**</span><span class="sxs-lookup"><span data-stu-id="7626b-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="7626b-106">Klicka **på Webbplatssamlingens** funktioner under **Administration av webbplatssamling.**</span><span class="sxs-lookup"><span data-stu-id="7626b-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="7626b-107">Klicka på **Inaktivera bredvid nedlåst behörighetsläge för användare** med begränsad **åtkomst.**</span><span class="sxs-lookup"><span data-stu-id="7626b-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="7626b-108">Ett meddelande om nekad åtkomst kan också inträffa för delade mappar om webbplatsen är en publiceringswebbplats.</span><span class="sxs-lookup"><span data-stu-id="7626b-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="7626b-109">Mer information finns i [Åtkomst nekad när du öppnar en delad mapp.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="7626b-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="7626b-110">Om någon fick meddelandet "Åtkomst nekad" när han eller hon försöker visa åtkomstförfrågningar måste användaren läggas till som antingen administratör för webbplatssamlingen eller medlem i gruppen Ägare för webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="7626b-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="7626b-111">Mer information finns i listan [Åtkomst nekad till åtkomstbegäranden.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="7626b-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="7626b-112">Om en användare fick meddelandet "Åtkomst nekad" när de togs bort från Active Directory lokalt och sedan lades till igen, se Åtkomst nekad när ett användarkonto synkroniseras till [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="7626b-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

