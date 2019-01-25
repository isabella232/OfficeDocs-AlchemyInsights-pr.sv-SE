---
title: 932 uppgradera AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492540"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="78bf9-102">Uppgradering av Azure AD Anslut</span><span class="sxs-lookup"><span data-stu-id="78bf9-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="78bf9-p101">Som standard aktiveras automatisk uppgradering för Azure AD Connect, som hjälper till att se till att du kör den senaste versionen. Om du vill kontrollera inställningarna för automatisk uppgradering använder du cmdlet **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdlet returnerar ett av följande värden:</span><span class="sxs-lookup"><span data-stu-id="78bf9-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="78bf9-106">**Aktiverad**: automatisk uppgradering är aktiverad.</span><span class="sxs-lookup"><span data-stu-id="78bf9-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="78bf9-107">**Inaktiverad**: automatisk uppgradering har inaktiverats.</span><span class="sxs-lookup"><span data-stu-id="78bf9-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="78bf9-p102">**Suspended**: systemet inte längre är berättigad till automatiska uppgraderingar. Du kan inte konfigurera den här värde. den anges av systemet.</span><span class="sxs-lookup"><span data-stu-id="78bf9-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="78bf9-110">Mer information finns i [automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="78bf9-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="78bf9-111">Om du vill hämta den senaste versionen av Azure AD Connect, gå till [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="78bf9-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

