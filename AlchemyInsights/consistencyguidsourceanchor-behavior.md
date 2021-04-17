---
title: ConsistencyGuid/sourceAnchor-beteende
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817010"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-beteende

Azure AD Connect (version 1.1.524.0 och senare) underlättar nu användningen av msDS-ConsistencyGuid som sourceAnchor-attribut. När du använder den här funktionen konfigurerar Azure AD Connect automatiskt synkroniseringsreglerna till:
  
- Använd msDS-ConsistencyGuid som attributet sourceAnchor för användarobjekt. ObjectGUID används för andra objekttyper.
    
- För alla lokala AD-användarobjekt med msDS-ConsistencyGuid-attributet som inte fylls i skriver Azure AD Connect sitt objectGUID-värde tillbaka till attributet msDS-ConsistencyGuid i den lokala Active Directory. När attributet msDS-ConsistencyGuid har fyllts i exporterar Azure AD Connect sedan objektet till Azure AD.
    
 **Obs!** När ett lokalt AD-objekt importerats till Azure AD Connect (d.v.s. importerats till AD-anslutningsutrymmet och projicerats till metaversumet) kan du inte längre ändra dess sourceAnchor-värde. Om du vill ange värdet sourceAnchor för ett visst lokalt AD-objekt konfigurerar du attributet msDS-ConsistencyGuid innan det importeras till Azure AD Connect. 
  
Mer information om SourceAnchor och ConsistencyGuid finns i följande avsnitt: [Azure AD Connect: Designkoncept](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

