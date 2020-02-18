---
title: Det går inte att ange eller visa policyn AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091774"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="9267d-102">Det går inte att ange eller visa policyn AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="9267d-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="9267d-103">När du försöker ange eller visa allowSelfServicePurchase-principen visas följande felmeddelande:</span><span class="sxs-lookup"><span data-stu-id="9267d-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="9267d-104">*HandleError : Det gick inte att hämta produktprincipen med PolicyId 'AllowSelfServicePurchase', ErrorMessage - Den underliggande anslutningen stängdes: Ett oväntat fel uppstod på ett skicka.*</span><span class="sxs-lookup"><span data-stu-id="9267d-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="9267d-105">Detta kan bero på en äldre version av Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="9267d-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="9267d-106">Om du vill ansluta MSCommerce-tjänsten måste du använda TLS 1.2 eller större.</span><span class="sxs-lookup"><span data-stu-id="9267d-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="9267d-107">Prova följande steg för att aktivera/ange TLS-protokollet till 1.2, verifiera och försök igen.</span><span class="sxs-lookup"><span data-stu-id="9267d-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="9267d-108">Vid kommandotolken för PowerShell\) (PS C: ange följande kommando för att ställa in TLS-protokollet till version 1.2:</span><span class="sxs-lookup"><span data-stu-id="9267d-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="9267d-109">\[Net.ServicePointManager]:SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="9267d-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="9267d-110">Kontrollera att TLS-protokollen används, med följande kommando:</span><span class="sxs-lookup"><span data-stu-id="9267d-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="9267d-111">\[Net.ServicePointManager]:SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="9267d-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="9267d-112">Försök igen kommandonhämta eller uppdatera efter behov.</span><span class="sxs-lookup"><span data-stu-id="9267d-112">Retry the Get or Update commands as needed.</span></span>

