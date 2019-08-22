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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517013"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor beteende

Azure AD Connect (version 1.1.524.0 och efter) nu förenklar användningen av msDS-ConsistencyGuid som sourceAnchor attribut. När du använder den här funktionen konfigurerar Azure AD Anslut automatiskt Synkroniseringsregler:
  
- Använd msDS-ConsistencyGuid som sourceAnchor attribut för användarobjekt. ObjectGUID används för andra objekttyper.
    
- För alla angivna lokal AD-användare objekt vars attributet msDS-ConsistencyGuid är inte ifyllda, Azure AD Anslut skrivningar objectGUID värdet tillbaka till attributet msDS-ConsistencyGuid i lokal Active Directory. När attributet msDS-ConsistencyGuid fylls exporterar Azure AD Anslut sedan objektet till Azure AD.
    
 **Observera:** När en lokal AD-objekt importeras till Azure AD Connect (som kan importeras till AD Anslutningsområde och planerat in metaversumsökningen), du kan inte längre ändra dess värde för sourceAnchor. Ange sourceAnchor-värdet för en ges lokal AD objekt, konfigurera ett attributet msDS-ConsistencyGuid innan den importeras till Azure AD Connect. 
  
Mer information om SourceAnchor och ConsistencyGuid finns följande: [Azure AD Anslut: utforma begrepp](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

