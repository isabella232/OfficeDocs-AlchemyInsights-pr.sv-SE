---
title: Fel AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709169"
---
# <a name="error-attributevaluemustbeunique"></a>Fel: AttributeValueMustBeUnique

Den vanligaste orsaken till AttributeValueMustBeUnique-felet är att två objekt med olika SourceAnchor (immutableId) har samma värde för attributen ProxyAddresses och/eller UserPrincipalName. Så här löser du AttributeValueMustBeUnique-felet:
  
1. Identifiera det duplicerade proxyAddresses, userPrincipalName eller ett annat attributvärde som orsakar felet. Identifiera också vilka två (eller fler) objekt som är involverade i konflikten. Den rapport som genereras av Azure AD Connect-hälsa för synkronisering kan hjälpa dig att identifiera de två objekten.
    
2. Identifiera vilket objekt som ska fortsätta ha det duplicerade värdet och vilket objekt som inte ska användas.
    
3. Ta bort det duplicerade värdet från objektet som inte ska ha det värdet. Observera att du bör göra ändringarna i den katalog där objektet har en källa från. I vissa fall kan du behöva ta bort ett av objekten i konflikt.
    
4. Om du har gjort ändringen i den lokala ANNONSen kan Azure AD Connect-synkroniseringen för att åtgärda felet åtgärdas.
    

