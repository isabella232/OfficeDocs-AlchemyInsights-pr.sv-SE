---
title: Det går inte att ange eller Visa AllowSelfServicePurchase policy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735217"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="c98fc-102">Det går inte att ange eller Visa AllowSelfServicePurchase policy</span><span class="sxs-lookup"><span data-stu-id="c98fc-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="c98fc-103">När du försöker ange eller Visa AllowSelfServicePurchase policy visas följande fel meddelande:</span><span class="sxs-lookup"><span data-stu-id="c98fc-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="c98fc-104">*HandleError: det gick inte att hämta produkt princip med PolicyId ' AllowSelfServicePurchase ', ErrorMessage-den underliggande anslutningen avslutades: ett oväntat fel uppstod vid sändning.*</span><span class="sxs-lookup"><span data-stu-id="c98fc-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="c98fc-105">Detta kan bero på att en äldre version av Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="c98fc-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="c98fc-106">För att kunna ansluta MSCommerce-tjänsten måste du använda TLS 1,2 eller senare.</span><span class="sxs-lookup"><span data-stu-id="c98fc-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="c98fc-107">Prova följande steg för att aktivera/ange TLS-protokollet till 1,2, verifiera och försök igen.</span><span class="sxs-lookup"><span data-stu-id="c98fc-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="c98fc-108">I kommando tolken för PowerShell (PS C: \) Ange följande kommando för att ange TLS-protokollet till version 1,2:</span><span class="sxs-lookup"><span data-stu-id="c98fc-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="c98fc-109">Verifiera vilka TLS-protokoll som används, med följande kommando:</span><span class="sxs-lookup"><span data-stu-id="c98fc-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="c98fc-110">Försök hämta eller uppdatera kommandona igen.</span><span class="sxs-lookup"><span data-stu-id="c98fc-110">Retry the Get or Update commands as needed.</span></span>

