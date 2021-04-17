---
title: Felsökning av säkerhetstips vid identifiering av bedrägerier
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834749"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="826a3-102">Felsökning av säkerhetstips vid identifiering av bedrägerier</span><span class="sxs-lookup"><span data-stu-id="826a3-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="826a3-103">Om du får ett säkerhetstips där det står "Avsändaren misslyckades med våra kontroller för identifiering av bedrägerier och kanske inte är den som de verkar vara", så gick det inte att överföra antingen DKIM- eller SPF-autentiseringskontrollerna till avsändaren.</span><span class="sxs-lookup"><span data-stu-id="826a3-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="826a3-104">Den bästa metoden för att lösa det här är att avsändaren godkänner sig själv.</span><span class="sxs-lookup"><span data-stu-id="826a3-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="826a3-105">Om avsändaren skickar åt dig måste du auktorisera dem genom att lägga till avsändarens IP-adress till SPF-posten.</span><span class="sxs-lookup"><span data-stu-id="826a3-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="826a3-106">Mer [information finns i Felsökning av röda (misstänkta) säkerhetstips](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) för identifiering av bedrägerier.</span><span class="sxs-lookup"><span data-stu-id="826a3-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="826a3-107">Här är några andra länkar som kan vara till hjälp:</span><span class="sxs-lookup"><span data-stu-id="826a3-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="826a3-108">Hur Microsoft använder Sender Policy Framework (SPF) för att förhindra förfalskning</span><span class="sxs-lookup"><span data-stu-id="826a3-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="826a3-109">Konfigurera SPF för att förhindra förfalskning</span><span class="sxs-lookup"><span data-stu-id="826a3-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
