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
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527069"
---
# <a name="error-attributevaluemustbeunique"></a>Fel: AttributeValueMustBeUnique

Den vanligaste orsaken till felet i AttributeValueMustBeUnique är två objekt med olika SourceAnchor (immutableId) har samma värde för attributen ProxyAddresses eller UserPrincipalName. Korrigera felet AttributeValueMustBeUnique:
  
1. Identifiera dubbletter proxyAddresses, userPrincipalName eller andra attributvärde som orsakar felet. Också identifiera vilka två (eller fler) objekt som är inblandade i konflikten. Rapporten som genereras av Azure AD ansluta hälsa för synkronisering kan hjälpa dig att identifiera de två objekten.
    
2. Identifiera vilka objekt bör fortsätta att ha duplicerade värde och vilket objekt bör inte.
    
3. Ta bort duplicerade värde från objekt som inte ska ha värdet. Observera att du bör göra en ändring i katalogen där objektet ursprung i. I vissa fall kan du behöva ta bort ett objekt i konflikt.
    
4. Om du har gjort ändringen i lokaler på AD kan Azure AD Anslut synkronisera ändring för fel som får fastställas.
    

