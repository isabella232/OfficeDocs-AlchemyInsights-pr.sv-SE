---
title: Fel AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499652"
---
# <a name="error-attributevaluemustbeunique"></a>Fel: AttributeValueMustBeUnique

Den vanligaste orsaken till felet i AttributeValueMustBeUnique är två objekt med olika SourceAnchor (immutableId) har samma värde för attributen ProxyAddresses eller UserPrincipalName. Korrigera felet AttributeValueMustBeUnique:
  
1. Identifiera dubbletter proxyAddresses, userPrincipalName eller andra attributvärde som orsakar felet. Också identifiera vilka två (eller fler) objekt som är inblandade i konflikten. Rapporten som genereras av Azure AD ansluta hälsa för synkronisering kan hjälpa dig att identifiera de två objekten.
    
2. Identifiera vilka objekt bör fortsätta att ha duplicerade värde och vilket objekt bör inte.
    
3. Ta bort duplicerade värde från objekt som inte ska ha värdet. Observera att du bör göra en ändring i katalogen där objektet ursprung i. I vissa fall kan du behöva ta bort ett objekt i konflikt.
    
4. Om du har gjort ändringen i lokaler på AD kan Azure AD Anslut synkronisera ändring för fel som får fastställas.
    

