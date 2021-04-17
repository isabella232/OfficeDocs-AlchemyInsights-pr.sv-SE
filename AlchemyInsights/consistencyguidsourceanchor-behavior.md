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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="8c9f9-102">ConsistencyGuid/sourceAnchor-beteende</span><span class="sxs-lookup"><span data-stu-id="8c9f9-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="8c9f9-103">Azure AD Connect (version 1.1.524.0 och senare) underlättar nu användningen av msDS-ConsistencyGuid som sourceAnchor-attribut.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="8c9f9-104">När du använder den här funktionen konfigurerar Azure AD Connect automatiskt synkroniseringsreglerna till:</span><span class="sxs-lookup"><span data-stu-id="8c9f9-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="8c9f9-105">Använd msDS-ConsistencyGuid som attributet sourceAnchor för användarobjekt.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="8c9f9-106">ObjectGUID används för andra objekttyper.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="8c9f9-107">För alla lokala AD-användarobjekt med msDS-ConsistencyGuid-attributet som inte fylls i skriver Azure AD Connect sitt objectGUID-värde tillbaka till attributet msDS-ConsistencyGuid i den lokala Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="8c9f9-108">När attributet msDS-ConsistencyGuid har fyllts i exporterar Azure AD Connect sedan objektet till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="8c9f9-109">**Obs!** När ett lokalt AD-objekt importerats till Azure AD Connect (d.v.s. importerats till AD-anslutningsutrymmet och projicerats till metaversumet) kan du inte längre ändra dess sourceAnchor-värde.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="8c9f9-110">Om du vill ange värdet sourceAnchor för ett visst lokalt AD-objekt konfigurerar du attributet msDS-ConsistencyGuid innan det importeras till Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="8c9f9-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="8c9f9-111">Mer information om SourceAnchor och ConsistencyGuid finns i följande avsnitt: [Azure AD Connect: Designkoncept](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="8c9f9-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

