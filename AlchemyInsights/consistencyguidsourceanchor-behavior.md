---
title: ConsistencyGuid/sourceAnchor-beteende
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756301"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor-beteende

Azure AD Connect (version 1.1.524.0 och after) underlättar nu användning av attributet msDS-ConsistencyGuid as sourceAnchor. När du använder den här funktionen konfigurerar Azure AD Connect automatiskt synkroniseringsinställningarna till:
  
- Använd msDS-ConsistencyGuid som sourceAnchor-attribut för användar objekt. ObjectGUID används för andra objekt typer.
    
- För vissa lokala AD-användarkonton vars attributet msDS-ConsistencyGuid inte är ifyllt skriver Azure AD Connect sitt objectGUID-värde till attributet msDS-ConsistencyGuid i lokala Active Directory. När attributet msDS-ConsistencyGuid har fyllts exporterar Azure AD Connect objektet till Azure AD.
    
 **Obs!** När ett lokalt AD-objekt importeras till Azure AD Connect (d.v.s. importeras till AD Connector-utrymmet och projiceras i metaverse) kan du inte längre ändra dess sourceAnchor-värde. Om du vill ange sourceAnchor-värdet för ett visst lokalt AD-objekt konfigurerar du attributet msDS-ConsistencyGuid innan det importeras till Azure AD Connect. 
  
Mer information om SourceAnchor och ConsistencyGuid finns i följande avsnitt: [Azure AD Connect: design koncept](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

