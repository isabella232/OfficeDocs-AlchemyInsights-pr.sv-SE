---
title: UPN-synkronisering avaktiverad
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749532"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="f158b-102">UPN-synkronisering avaktiverad</span><span class="sxs-lookup"><span data-stu-id="f158b-102">UPN sync disabled</span></span>

<span data-ttu-id="f158b-103">Om du började synkronisera med Azure AD före 30 mars 2016 kör du följande Azure AD PowerShell-cmdlet för att aktivera automatisk nedladdning av UPN för din organisation:</span><span class="sxs-lookup"><span data-stu-id="f158b-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="f158b-104">**Set-MsolDirSyncFeature-EnableSoftMatchOnUpn-aktivera $True**</span><span class="sxs-lookup"><span data-stu-id="f158b-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="f158b-105">Den mjuka UPN-matchningen aktive ras automatiskt för organisationer som startade synkronisering till Azure AD den 30 mars 2016 eller senare.</span><span class="sxs-lookup"><span data-stu-id="f158b-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="f158b-106">Om du vill veta mer om hur du aktiverar mjuk matchning på UPN och andra synkroniseringskopplingar kan du läsa mer i [Azure AD Connect Sync service-funktionerna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="f158b-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

