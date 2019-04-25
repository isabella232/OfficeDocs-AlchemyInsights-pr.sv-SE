---
title: ConsistencyGuid / sourceAnchor beteende
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
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408126"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor beteende

Azure AD Connect (version 1.1.524.0 och efter) nu förenklar användningen av msDS-ConsistencyGuid som sourceAnchor attribut. När du använder den här funktionen konfigurerar Azure AD Anslut automatiskt Synkroniseringsregler:
  
- Använd msDS-ConsistencyGuid som sourceAnchor attribut för användarobjekt. ObjectGUID används för andra objekttyper.
    
- För alla angivna lokal AD-användare objekt vars attributet msDS-ConsistencyGuid är inte ifyllda, Azure AD Anslut skrivningar objectGUID värdet tillbaka till attributet msDS-ConsistencyGuid i lokal Active Directory. När attributet msDS-ConsistencyGuid fylls exporterar Azure AD Anslut sedan objektet till Azure AD.
    
 **Observera:** När en lokal AD-objekt importeras till Azure AD Connect (som kan importeras till AD Anslutningsområde och planerat in metaversumsökningen), du kan inte längre ändra dess värde för sourceAnchor. Ange sourceAnchor-värdet för en ges lokal AD objekt, konfigurera ett attributet msDS-ConsistencyGuid innan den importeras till Azure AD Connect. 
  
Mer information om SourceAnchor och ConsistencyGuid finns följande: [Azure AD Anslut: utforma begrepp](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

