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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044359"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-beteende

Azure AD Anslut (version 1.1.524.0 och senare) underlättar nu användningen av msDS-ConsistencyGuid som sourceAnchor-attribut. När du använder den här funktionen Anslut Azure AD automatiskt synkroniseringsreglerna till att:
  
- Använd msDS-ConsistencyGuid som attributet sourceAnchor för användarobjekt. ObjectGUID används för andra objekttyper.
    
- För alla lokala AD-användarobjekt med msDS-ConsistencyGuid-attributet som inte fylls i skriver Azure AD Anslut sitt objectGUID-värde tillbaka till attributet msDS-ConsistencyGuid i lokalt Active Directory. När attributet msDS-ConsistencyGuid har fyllts i exporterar Azure AD Anslut objektet till Azure AD.
    
 **Obs!** När ett lokalt AD-objekt importerats till Azure AD Anslut (d.v.s. importerats till AD-anslutningsutrymmet och projicerats till metaversumet) kan du inte ändra dess sourceAnchor-värde längre. Om du vill ange värdet sourceAnchor för ett visst lokalt AD-objekt konfigurerar du attributet msDS-ConsistencyGuid innan det importeras till Azure AD Anslut. 
  
Mer information om SourceAnchor och ConsistencyGuid finns i följande avsnitt: [Azure AD Anslut: Designkoncept](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

