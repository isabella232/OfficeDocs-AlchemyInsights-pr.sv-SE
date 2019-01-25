---
title: ConsistencyGuid / sourceAnchor beteende
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498536"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="3b475-102">ConsistencyGuid / sourceAnchor beteende</span><span class="sxs-lookup"><span data-stu-id="3b475-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="3b475-p101">Azure AD Connect (version 1.1.524.0 och efter) nu förenklar användningen av msDS-ConsistencyGuid som sourceAnchor attribut. När du använder den här funktionen konfigurerar Azure AD Anslut automatiskt Synkroniseringsregler:</span><span class="sxs-lookup"><span data-stu-id="3b475-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="3b475-p102">Använd msDS-ConsistencyGuid som sourceAnchor attribut för användarobjekt. ObjectGUID används för andra objekttyper.</span><span class="sxs-lookup"><span data-stu-id="3b475-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="3b475-p103">För alla angivna lokal AD-användare objekt vars attributet msDS-ConsistencyGuid är inte ifyllda, Azure AD Anslut skrivningar objectGUID värdet tillbaka till attributet msDS-ConsistencyGuid i lokal Active Directory. När attributet msDS-ConsistencyGuid fylls exporterar Azure AD Anslut sedan objektet till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b475-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="3b475-p104">**Observera:** När en lokal AD-objekt importeras till Azure AD Connect (som kan importeras till AD Anslutningsområde och planerat in metaversumsökningen), du kan inte längre ändra dess värde för sourceAnchor. Ange sourceAnchor-värdet för en ges lokal AD objekt, konfigurera ett attributet msDS-ConsistencyGuid innan den importeras till Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3b475-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="3b475-111">Mer information om SourceAnchor och ConsistencyGuid finns följande: [Azure AD Anslut: utforma begrepp](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="3b475-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

