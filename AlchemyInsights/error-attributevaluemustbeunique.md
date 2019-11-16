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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/15/2019
ms.locfileid: "36527069"
---
# <a name="error-attributevaluemustbeunique"></a>Fel: AttributeValueMustBeUnique

Den vanligaste orsaken till felet AttributeValueMustBeUnique är två objekt med olika SourceAnchor (immutableId) har samma värde för attributen ProxyAddresses och/eller UserPrincipalName. Så här åtgärdar du AttributeValueMustBeUnique-felet:
  
1. Identifiera duplicerade proxyAddresses, userPrincipalName eller andra attributvärde som orsakar felet. Identifiera också vilka två (eller fler) objekt som är inblandade i konflikten. Rapporten som genereras av Azure AD Connect Health för synkronisering kan hjälpa dig att identifiera de två objekten.
    
2. Identifiera vilket objekt som ska fortsätta att ha duplicerat värde och vilket objekt som inte ska.
    
3. Ta bort duplicerade värdet från objektet som inte ska ha det värdet. Observera att du bör göra ändringen i katalogen där objektet hämtas från. I vissa fall kan du behöva ta bort ett av objekten i konflikt.
    
4. Om du har gjort ändringen i lokal AD, låt Azure AD Connect synkronisera ändringen för felet att få fast.
    

