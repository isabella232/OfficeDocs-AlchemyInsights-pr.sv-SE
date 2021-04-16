---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813778"
---
# <a name="error-attributevaluemustbeunique"></a>Fel: AttributeValueMustBeUnique

Den vanligaste orsaken till AttributeValueMustBeUnique-felet är två objekt med olika SourceAnchor (immutableId) har samma värde för ProxyAddresses- och/eller UserPrincipalName-attributen. Så här åtgärdar du attributeValueMustBeUnique-felet:
  
1. Identifiera det duplicerade proxyAddresses-, userPrincipalName- eller annat attributvärde som orsakar felet. Identifiera även vilka (eller flera) objekt som är inblandade i konflikten. Rapporten som genereras av Azure AD Connect Health för synkronisering kan hjälpa dig att identifiera de två objekten.
    
2. Identifiera vilket objekt som ska ha det duplicerade värdet och vilket objekt som inte ska ha det.
    
3. Ta bort det duplicerade värdet från objektet som INTE ska ha det värdet. Observera att du bör göra ändringen i katalogen där objektet kommer från. I vissa fall kan du behöva ta bort något av objekten i konflikt.
    
4. Om du har gjort ändringen i lokal AD kan du låta Azure AD Connect synkronisera ändringen för att åtgärda felet.
    

