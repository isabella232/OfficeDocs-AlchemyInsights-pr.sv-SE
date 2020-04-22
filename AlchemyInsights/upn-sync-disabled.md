---
title: UPN-synkronisering inaktiverad
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726122"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering inaktiverad

Om du började synkronisera med Azure AD före den 30 mars 2016 kör du följande Azure AD PowerShell-cmdlet för att aktivera UPN mjuk matchning endast för din organisation:
  
 **Set-MsolDirSyncFeature -Funktionen EnableSoftMatchOnUpn -Aktivera $True**
  
UPN soft match aktiveras automatiskt för organisationer som började synkroniseras med Azure AD på eller efter den 30 mars 2016.
  
Mer information om hur du aktiverar mjuk matchning på UPN och andra synkroniseringsfunktioner finns i [Azure AD Connect-synkroniseringstjänstfunktioner](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

