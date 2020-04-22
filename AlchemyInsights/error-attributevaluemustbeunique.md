---
title: FelattributVärdeMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703192"
---
# <a name="error-attributevaluemustbeunique"></a>Fel: AttributeValueMustBeUnique

Den vanligaste orsaken till attributevalueMustBeUnique-felet är två objekt med olika SourceAnchor (oföränderligId) har samma värde för attributet ProxyAddresses och/eller UserPrincipalName. Så här åtgärdar du attributevalueMustBeUnique-felet:
  
1. Identifiera de duplicerade proxyadresserna, userPrincipalName eller något annat attributvärde som orsakar felet. Identifiera också vilka två (eller flera) objekt som är inblandade i konflikten. Rapporten som genereras av Azure AD Connect Health för synkronisering kan hjälpa dig att identifiera de två objekten.
    
2. Identifiera vilket objekt som ska fortsätta att ha det duplicerade värdet och vilket objekt som inte ska.
    
3. Ta bort det duplicerade värdet från objektet som INTE ska ha det värdet. Observera att du bör göra ändringen i katalogen där objektet kommer från. I vissa fall kan du behöva ta bort ett av objekten i konflikt.
    
4. Om du har gjort ändringen i den lokala AD:en låter du Azure AD Connect synkronisera ändringen för att felet ska åtgärdas.
    

