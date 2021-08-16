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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002142"
---
# <a name="error-attributevaluemustbeunique"></a>Fel: AttributeValueMustBeUnique

Den vanligaste orsaken till AttributeValueMustBeUnique-felet är två objekt med olika SourceAnchor (immutableId) har samma värde för ProxyAddresses- och/eller UserPrincipalName-attributen. Så här åtgärdar du attributeValueMustBeUnique-felet:
  
1. Identifiera det duplicerade proxyAddresses-, userPrincipalName- eller annat attributvärde som orsakar felet. Identifiera även vilka (eller flera) objekt som är inblandade i konflikten. Rapporten som genereras av Azure AD Anslut För synkronisering kan hjälpa dig att identifiera de två objekten.
    
2. Identifiera vilket objekt som ska ha det duplicerade värdet och vilket objekt som inte ska ha det.
    
3. Ta bort det duplicerade värdet från objektet som INTE ska ha det värdet. Observera att du bör göra ändringen i katalogen där objektet kommer från. I vissa fall kan du behöva ta bort något av objekten i konflikt.
    
4. Om du har gjort ändringen i lokal AD kan du låta Azure AD Anslut för att åtgärda felet.
    

