---
title: 1554 Winsock-fel 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492419"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="15b1d-102">Winsock-fel 10061</span><span class="sxs-lookup"><span data-stu-id="15b1d-102">Winsock error 10061</span></span>

<span data-ttu-id="15b1d-p101">Felet innebär att Office 365 gick inte att upprätta en TCP-socket (anslutning) med målvärden. Den mest troliga orsaken till detta fel är ett problem med konfigurationen av brandväggen. Åtgärda problemet genom att kontrollera inställningarna:</span><span class="sxs-lookup"><span data-stu-id="15b1d-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="15b1d-106">Kontrollera konfigurationen av brandväggen med informationen i [Office 365-adresser och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="15b1d-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="15b1d-107">Om felet är specifikt till Exchange Online skydd (EOP), bör du tidigare anmälts till en ändring till [Exchange Online skydd IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="15b1d-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="15b1d-108">Kontrollera att porten inte blockering av Internet Service Provider (ISP).</span><span class="sxs-lookup"><span data-stu-id="15b1d-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="15b1d-109">Kontrollera smart värd- och måldator-serverinställningarna i kopplingar.</span><span class="sxs-lookup"><span data-stu-id="15b1d-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="15b1d-110">Observera att Office 365 inte blockerar *inkommande* anslutningar på detta sätt.</span><span class="sxs-lookup"><span data-stu-id="15b1d-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

