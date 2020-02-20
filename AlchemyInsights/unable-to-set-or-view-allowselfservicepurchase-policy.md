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
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158579"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="765b2-102">Det går inte att ange eller visa policyn AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="765b2-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="765b2-103">När du försöker ange eller visa allowSelfServicePurchase-principen visas följande felmeddelande:</span><span class="sxs-lookup"><span data-stu-id="765b2-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="765b2-104">*HandleError : Det gick inte att hämta produktprincipen med PolicyId 'AllowSelfServicePurchase', ErrorMessage - Den underliggande anslutningen stängdes: Ett oväntat fel uppstod på ett skicka.*</span><span class="sxs-lookup"><span data-stu-id="765b2-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="765b2-105">Detta kan bero på en äldre version av Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="765b2-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="765b2-106">Om du vill ansluta MSCommerce-tjänsten måste du använda TLS 1.2 eller större.</span><span class="sxs-lookup"><span data-stu-id="765b2-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="765b2-107">Prova följande steg för att aktivera/ange TLS-protokollet till 1.2, verifiera och försök igen.</span><span class="sxs-lookup"><span data-stu-id="765b2-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="765b2-108">Vid kommandotolken för PowerShell\) (PS C: ange följande kommando för att ställa in TLS-protokollet till version 1.2:</span><span class="sxs-lookup"><span data-stu-id="765b2-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="765b2-109">Kontrollera att TLS-protokollen används, med följande kommando:</span><span class="sxs-lookup"><span data-stu-id="765b2-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="765b2-110">Försök igen kommandonhämta eller uppdatera efter behov.</span><span class="sxs-lookup"><span data-stu-id="765b2-110">Retry the Get or Update commands as needed.</span></span>

