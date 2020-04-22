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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="15ae1-102">ConsistencyGuid / sourceAnchor beteende</span><span class="sxs-lookup"><span data-stu-id="15ae1-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="15ae1-103">Azure AD Connect (version 1.1.524.0 och efter) underlättar nu användningen av msDS-ConsistencyGuid som sourceAnchor-attribut.</span><span class="sxs-lookup"><span data-stu-id="15ae1-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="15ae1-104">När du använder den här funktionen konfigurerar Azure AD Connect automatiskt synkroniseringsreglerna till:</span><span class="sxs-lookup"><span data-stu-id="15ae1-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="15ae1-105">Använd msDS-ConsistencyGuid som sourceAnchor-attribut för användarobjekt.</span><span class="sxs-lookup"><span data-stu-id="15ae1-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="15ae1-106">ObjectGUID används för andra objekttyper.</span><span class="sxs-lookup"><span data-stu-id="15ae1-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="15ae1-107">För ett givet lokalt AD-användarobjekt vars msDS-ConsistencyGuid-attribut inte är ifyllt skriver Azure AD Connect tillbaka sitt objectGUID-värde till attributet msDS-ConsistencyGuid i lokal Active Directory.</span><span class="sxs-lookup"><span data-stu-id="15ae1-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="15ae1-108">När attributet msDS-ConsistencyGuid har fyllts i exporterar Azure AD Connect objektet till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="15ae1-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="15ae1-109">**Anm.:** När ett lokalt AD-objekt har importerats till Azure AD Connect (det vill säga importeras till AD-anslutningsutrymmet och projiceras till Metaverse) kan du inte längre ändra dess sourceAnchor-värde.</span><span class="sxs-lookup"><span data-stu-id="15ae1-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="15ae1-110">Om du vill ange sourceAnchor-värdet för ett givet lokalt AD-objekt konfigurerar du attributet msDS-ConsistencyGuid innan det importeras till Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="15ae1-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="15ae1-111">Mer information om SourceAnchor och ConsistencyGuid finns i följande avsnitt: [Azure AD Connect: Design-koncept](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="15ae1-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

