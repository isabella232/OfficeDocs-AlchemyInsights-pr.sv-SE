---
title: UPN-synkronisering har inaktiverats
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492304"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering har inaktiverats

Kör följande Azure AD PowerShell-cmdlet om du vill aktivera UPN-soft passar organisationen endast om du har startats synkroniseras med Azure AD före den 30 mars 2016:
  
 **Ange MsolDirSyncFeature-funktionen EnableSoftMatchOnUpn-aktivera $True**
  
UPN-mjuk matchning är automatiskt aktiverat för organisationer som har startats synkroniseras med Azure AD på eller efter den 30 mars 2016.
  
Mer information om hur du aktiverar mjuk matchar UPN och andra synkroniseringsfunktioner finns i [Azure AD Anslut synkroniseringsfunktioner för tjänsten](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

