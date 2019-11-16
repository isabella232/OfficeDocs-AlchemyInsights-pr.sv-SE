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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/15/2019
ms.locfileid: "36517013"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="dcdf6-102">ConsistencyGuid/sourceAnchor beteende</span><span class="sxs-lookup"><span data-stu-id="dcdf6-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="dcdf6-103">Azure AD Connect (version 1.1.524.0 och senare) nu underlättar användningen av msDS-ConsistencyGuid som sourceAnchor-attribut.</span><span class="sxs-lookup"><span data-stu-id="dcdf6-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="dcdf6-104">När du använder den här funktionen konfigurerar Azure AD Connect automatiskt synkroniseringsreglerna till:</span><span class="sxs-lookup"><span data-stu-id="dcdf6-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="dcdf6-105">Använd msDS-ConsistencyGuid som sourceAnchor-attribut för användarobjekt.</span><span class="sxs-lookup"><span data-stu-id="dcdf6-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="dcdf6-106">ObjectGUID används för andra objekttyper.</span><span class="sxs-lookup"><span data-stu-id="dcdf6-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="dcdf6-107">För alla angivna lokala AD-användarobjekt vars msDS-ConsistencyGuid-attributet inte fylls i Azure AD Connect skriver sitt objectGUID-värde tillbaka till attributet msDS-ConsistencyGuid i den lokala Active Directory.</span><span class="sxs-lookup"><span data-stu-id="dcdf6-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="dcdf6-108">När attributet msDS-ConsistencyGuid fylls, exporterar Azure AD Connect sedan objektet till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dcdf6-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="dcdf6-109">**Anmärkning:** När ett lokalt AD-objekt importeras till Azure AD Connect (som importeras till AD Connector-utrymmet och projiceras i metaversum), kan du inte ändra dess sourceAnchor-värde längre.</span><span class="sxs-lookup"><span data-stu-id="dcdf6-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="dcdf6-110">Om du vill ange sourceAnchor-värdet för ett visst lokalt AD-objekt, konfigurera dess msDS-ConsistencyGuid attribut innan den importeras till Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="dcdf6-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="dcdf6-111">Mer information om SourceAnchor och ConsistencyGuid finns i följande: [Azure AD Connect: design koncept](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="dcdf6-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

