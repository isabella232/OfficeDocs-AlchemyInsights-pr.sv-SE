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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038130"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering inaktiverad

Om du började synkronisera till Azure AD före den 30 mars 2016 kör du följande Azure AD PowerShell-cmdlet för att aktivera UPN endast mjuk matchning för organisationen:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Mjuk UPN-matchning aktiveras automatiskt för organisationer som startade synkroniseringen med Azure AD den 30 mars 2016 eller senare.
  
Mer information om hur du aktiverar mjuk matchning på UPN och andra synkroniseringsfunktioner finns i [Azure AD Anslut för synkroniseringstjänsten.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

