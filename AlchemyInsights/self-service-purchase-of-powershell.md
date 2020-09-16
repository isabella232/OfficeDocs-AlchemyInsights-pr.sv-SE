---
title: Själv service köp av PowerShell
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
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739988"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="bd0be-102">Själv service köp av PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd0be-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="bd0be-103">För att använda MSCommerce PowerShell-modulen måste du installera den på en Windows 10-enhet med TLS 1,2 (lokal administratörs behörighet krävs).</span><span class="sxs-lookup"><span data-stu-id="bd0be-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="bd0be-104">Importera och Anslut till MSCommerce-modulen.</span><span class="sxs-lookup"><span data-stu-id="bd0be-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="bd0be-105">När du uppmanas att logga in måste du använda autentiseringsuppgifter för globala administratörer eller fakturerings administratör.</span><span class="sxs-lookup"><span data-stu-id="bd0be-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="bd0be-106">Om du inte har TLS 1,2 kan du få följande fel meddelande när du försöker hämta eller uppdatera principen:</span><span class="sxs-lookup"><span data-stu-id="bd0be-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="bd0be-107">*Errormessage-den underliggande anslutningen stängdes: ett oväntat fel uppstod vid sändning*.</span><span class="sxs-lookup"><span data-stu-id="bd0be-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



