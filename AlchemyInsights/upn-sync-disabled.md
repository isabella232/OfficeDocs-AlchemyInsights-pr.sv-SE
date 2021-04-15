---
title: UPN-synkronisering inaktiverad
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782169"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="74084-102">UPN-synkronisering inaktiverad</span><span class="sxs-lookup"><span data-stu-id="74084-102">UPN sync disabled</span></span>

<span data-ttu-id="74084-103">Om du började synkronisera till Azure AD före den 30 mars 2016 kör du följande Azure AD PowerShell-cmdlet för att aktivera UPN endast mjuk matchning för organisationen:</span><span class="sxs-lookup"><span data-stu-id="74084-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="74084-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="74084-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="74084-105">Mjuk UPN-matchning aktiveras automatiskt för organisationer som startade synkroniseringen med Azure AD den 30 mars 2016 eller senare.</span><span class="sxs-lookup"><span data-stu-id="74084-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="74084-106">Mer information om hur du aktiverar mjuk matchning på UPN och andra synkroniseringsfunktioner finns i [Azure AD Connect-synkroniseringstjänstens funktioner.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="74084-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

