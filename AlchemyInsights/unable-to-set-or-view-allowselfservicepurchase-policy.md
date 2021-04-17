---
title: Det går inte att ange eller visa principen AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826109"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="dce79-102">Det går inte att ange eller visa principen AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="dce79-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="dce79-103">När du försöker ange eller visa principen AllowSelfServicePurchase får du följande felmeddelande:</span><span class="sxs-lookup"><span data-stu-id="dce79-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="dce79-104">*HandleError: Det gick inte att hämta produktpolicy med PolicyId 'AllowSelfServicePurchase', ErrorMessage – Den underliggande anslutningen stängdes: Ett oväntat fel uppstod vid ett skicka-meddelande.*</span><span class="sxs-lookup"><span data-stu-id="dce79-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="dce79-105">Det här kan bero på en äldre version av TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="dce79-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="dce79-106">Du måste använda TLS 1.2 eller större för att ansluta tjänsten MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="dce79-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="dce79-107">Prova följande steg för att aktivera/ange TLS-protokollet till 1.2, verifiera och försök igen.</span><span class="sxs-lookup"><span data-stu-id="dce79-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="dce79-108">I PowerShell-kommandotolken (PS C: ange följande kommando för att ange \) TLS-protokollet till version 1.2:</span><span class="sxs-lookup"><span data-stu-id="dce79-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="dce79-109">Kontrollera det eller de TLS-protokoll som används, med följande kommando:</span><span class="sxs-lookup"><span data-stu-id="dce79-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="dce79-110">Försök igen med kommandona Hämta och Uppdatera efter behov.</span><span class="sxs-lookup"><span data-stu-id="dce79-110">Retry the Get or Update commands as needed.</span></span>

