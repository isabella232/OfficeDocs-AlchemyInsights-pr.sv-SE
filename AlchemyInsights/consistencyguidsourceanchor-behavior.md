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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="dd1e2-102">ConsistencyGuid/sourceAnchor-beteende</span><span class="sxs-lookup"><span data-stu-id="dd1e2-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="dd1e2-103">Azure AD Connect (version 1.1.524.0 och after) underlättar nu användning av attributet msDS-ConsistencyGuid as sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="dd1e2-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="dd1e2-104">När du använder den här funktionen konfigurerar Azure AD Connect automatiskt synkroniseringsinställningarna till:</span><span class="sxs-lookup"><span data-stu-id="dd1e2-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="dd1e2-105">Använd msDS-ConsistencyGuid som sourceAnchor-attribut för användar objekt.</span><span class="sxs-lookup"><span data-stu-id="dd1e2-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="dd1e2-106">ObjectGUID används för andra objekt typer.</span><span class="sxs-lookup"><span data-stu-id="dd1e2-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="dd1e2-107">För vissa lokala AD-användarkonton vars attributet msDS-ConsistencyGuid inte är ifyllt skriver Azure AD Connect sitt objectGUID-värde till attributet msDS-ConsistencyGuid i lokala Active Directory.</span><span class="sxs-lookup"><span data-stu-id="dd1e2-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="dd1e2-108">När attributet msDS-ConsistencyGuid har fyllts exporterar Azure AD Connect objektet till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dd1e2-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="dd1e2-109">**Obs!** När ett lokalt AD-objekt importeras till Azure AD Connect (d.v.s. importeras till AD Connector-utrymmet och projiceras i metaverse) kan du inte längre ändra dess sourceAnchor-värde.</span><span class="sxs-lookup"><span data-stu-id="dd1e2-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="dd1e2-110">Om du vill ange sourceAnchor-värdet för ett visst lokalt AD-objekt konfigurerar du attributet msDS-ConsistencyGuid innan det importeras till Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="dd1e2-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="dd1e2-111">Mer information om SourceAnchor och ConsistencyGuid finns i följande avsnitt: [Azure AD Connect: design koncept](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="dd1e2-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

