---
title: ConsistencyGuid/sourceAnchor beteende
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36517013"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor beteende

Azure AD Connect (version 1.1.524.0 och senare) nu underlättar användningen av msDS-ConsistencyGuid som sourceAnchor-attribut. När du använder den här funktionen konfigurerar Azure AD Connect automatiskt synkroniseringsreglerna till:
  
- Använd msDS-ConsistencyGuid som sourceAnchor-attribut för användarobjekt. ObjectGUID används för andra objekttyper.
    
- För alla angivna lokala AD-användarobjekt vars msDS-ConsistencyGuid-attributet inte fylls i Azure AD Connect skriver sitt objectGUID-värde tillbaka till attributet msDS-ConsistencyGuid i den lokala Active Directory. När attributet msDS-ConsistencyGuid fylls, exporterar Azure AD Connect sedan objektet till Azure AD.
    
 **Anmärkning:** När ett lokalt AD-objekt importeras till Azure AD Connect (som importeras till AD Connector-utrymmet och projiceras i metaversum), kan du inte ändra dess sourceAnchor-värde längre. Om du vill ange sourceAnchor-värdet för ett visst lokalt AD-objekt, konfigurera dess msDS-ConsistencyGuid attribut innan den importeras till Azure AD Connect. 
  
Mer information om SourceAnchor och ConsistencyGuid finns i följande: [Azure AD Connect: design koncept](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

