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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="7096c-102">ConsistencyGuid / sourceAnchor beteende</span><span class="sxs-lookup"><span data-stu-id="7096c-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="7096c-103">Azure AD Connect (version 1.1.524.0 och efter) nu förenklar användningen av msDS-ConsistencyGuid som sourceAnchor attribut.</span><span class="sxs-lookup"><span data-stu-id="7096c-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="7096c-104">När du använder den här funktionen konfigurerar Azure AD Anslut automatiskt Synkroniseringsregler:</span><span class="sxs-lookup"><span data-stu-id="7096c-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="7096c-105">Använd msDS-ConsistencyGuid som sourceAnchor attribut för användarobjekt.</span><span class="sxs-lookup"><span data-stu-id="7096c-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="7096c-106">ObjectGUID används för andra objekttyper.</span><span class="sxs-lookup"><span data-stu-id="7096c-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="7096c-107">För alla angivna lokal AD-användare objekt vars attributet msDS-ConsistencyGuid är inte ifyllda, Azure AD Anslut skrivningar objectGUID värdet tillbaka till attributet msDS-ConsistencyGuid i lokal Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7096c-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="7096c-108">När attributet msDS-ConsistencyGuid fylls exporterar Azure AD Anslut sedan objektet till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7096c-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="7096c-109">**Observera:** När en lokal AD-objekt importeras till Azure AD Connect (som kan importeras till AD Anslutningsområde och planerat in metaversumsökningen), du kan inte längre ändra dess värde för sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="7096c-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="7096c-110">Ange sourceAnchor-värdet för en ges lokal AD objekt, konfigurera ett attributet msDS-ConsistencyGuid innan den importeras till Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7096c-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="7096c-111">Mer information om SourceAnchor och ConsistencyGuid finns följande: [Azure AD Anslut: utforma begrepp](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="7096c-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

