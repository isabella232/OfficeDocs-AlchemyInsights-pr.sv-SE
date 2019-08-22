---
title: UPN-synkronisering har inaktiverats
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532349"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering har inaktiverats

Kör följande Azure AD PowerShell-cmdlet om du vill aktivera UPN-soft passar organisationen endast om du har startats synkroniseras med Azure AD före den 30 mars 2016:
  
 **Ange MsolDirSyncFeature-funktionen EnableSoftMatchOnUpn-aktivera $True**
  
UPN-mjuk matchning är automatiskt aktiverat för organisationer som har startats synkroniseras med Azure AD på eller efter den 30 mars 2016.
  
Mer information om hur du aktiverar mjuk matchar UPN och andra synkroniseringsfunktioner finns i [Azure AD Anslut synkroniseringsfunktioner för tjänsten](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

