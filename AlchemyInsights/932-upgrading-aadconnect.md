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
# <a name="upgrade-azure-ad-connect"></a>Uppgradering av Azure AD Anslut

Som standard aktiveras automatisk uppgradering för Azure AD Connect, som hjälper till att se till att du kör den senaste versionen. Om du vill kontrollera inställningarna för automatisk uppgradering använder du cmdlet **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdlet returnerar ett av följande värden: 
  
- **Aktiverad**: automatisk uppgradering är aktiverad. 
    
- **Inaktiverad**: automatisk uppgradering har inaktiverats. 
    
- **Suspended**: systemet inte längre är berättigad till automatiska uppgraderingar. Du kan inte konfigurera den här värde. den anges av systemet. 
    
Mer information finns i [automatisk uppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).
  
Om du vill hämta den senaste versionen av Azure AD Connect, gå till [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
  

