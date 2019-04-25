---
title: Fel AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402721"
---
# <a name="error-attributevaluemustbeunique"></a>Fel: AttributeValueMustBeUnique

Den vanligaste orsaken till felet i AttributeValueMustBeUnique är två objekt med olika SourceAnchor (immutableId) har samma värde för attributen ProxyAddresses eller UserPrincipalName. Korrigera felet AttributeValueMustBeUnique:
  
1. Identifiera dubbletter proxyAddresses, userPrincipalName eller andra attributvärde som orsakar felet. Också identifiera vilka två (eller fler) objekt som är inblandade i konflikten. Rapporten som genereras av Azure AD ansluta hälsa för synkronisering kan hjälpa dig att identifiera de två objekten.
    
2. Identifiera vilka objekt bör fortsätta att ha duplicerade värde och vilket objekt bör inte.
    
3. Ta bort duplicerade värde från objekt som inte ska ha värdet. Observera att du bör göra en ändring i katalogen där objektet ursprung i. I vissa fall kan du behöva ta bort ett objekt i konflikt.
    
4. Om du har gjort ändringen i lokaler på AD kan Azure AD Anslut synkronisera ändring för fel som får fastställas.
    

