---
title: ConsistencyGuid / sourceAnchor beteende
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705751"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor beteende

Azure AD Connect (version 1.1.524.0 och efter) underlättar nu användningen av msDS-ConsistencyGuid som sourceAnchor-attribut. När du använder den här funktionen konfigurerar Azure AD Connect automatiskt synkroniseringsreglerna till:
  
- Använd msDS-ConsistencyGuid som sourceAnchor-attribut för användarobjekt. ObjectGUID används för andra objekttyper.
    
- För ett givet lokalt AD-användarobjekt vars msDS-ConsistencyGuid-attribut inte är ifyllt skriver Azure AD Connect tillbaka sitt objectGUID-värde till attributet msDS-ConsistencyGuid i lokal Active Directory. När attributet msDS-ConsistencyGuid har fyllts i exporterar Azure AD Connect objektet till Azure AD.
    
 **Anm.:** När ett lokalt AD-objekt har importerats till Azure AD Connect (det vill säga importeras till AD-anslutningsutrymmet och projiceras till Metaverse) kan du inte längre ändra dess sourceAnchor-värde. Om du vill ange sourceAnchor-värdet för ett givet lokalt AD-objekt konfigurerar du attributet msDS-ConsistencyGuid innan det importeras till Azure AD Connect. 
  
Mer information om SourceAnchor och ConsistencyGuid finns i följande avsnitt: [Azure AD Connect: Design-koncept](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

