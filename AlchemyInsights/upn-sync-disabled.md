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
# <a name="upn-sync-disabled"></a>UPN-synkronisering avaktiverad

Om du började synkronisera med Azure AD före 30 mars 2016 kör du följande Azure AD PowerShell-cmdlet för att aktivera automatisk nedladdning av UPN för din organisation:
  
 **Set-MsolDirSyncFeature-EnableSoftMatchOnUpn-aktivera $True**
  
Den mjuka UPN-matchningen aktive ras automatiskt för organisationer som startade synkronisering till Azure AD den 30 mars 2016 eller senare.
  
Om du vill veta mer om hur du aktiverar mjuk matchning på UPN och andra synkroniseringskopplingar kan du läsa mer i [Azure AD Connect Sync service-funktionerna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

