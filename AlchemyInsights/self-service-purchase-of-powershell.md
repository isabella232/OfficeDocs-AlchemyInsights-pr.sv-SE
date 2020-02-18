---
title: Självbetjäningsköp av PowerShell
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
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091773"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="60cd1-102">Självbetjäningsköp av PowerShell</span><span class="sxs-lookup"><span data-stu-id="60cd1-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="60cd1-103">Om du vill använda MSCommerce PowerShell-modulen måste du installera den på en Windows 10-enhet med TLS 1.2 (lokala administratörsbehörigheter krävs).</span><span class="sxs-lookup"><span data-stu-id="60cd1-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="60cd1-104">Importera och anslut till MSCommerce-modulen.</span><span class="sxs-lookup"><span data-stu-id="60cd1-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="60cd1-105">När du uppmanas att logga in måste du använda rollautentiseringsuppgifter för globala eller faktureringsadministratörer.</span><span class="sxs-lookup"><span data-stu-id="60cd1-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="60cd1-106">Om du inte har TLS 1.2 kan du få följande fel när du försöker hämta eller uppdatera principen:</span><span class="sxs-lookup"><span data-stu-id="60cd1-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="60cd1-107">*ErrorMessage -Den underliggande anslutningen stängdes: Ett oväntat fel uppstod på en skicka*.</span><span class="sxs-lookup"><span data-stu-id="60cd1-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



