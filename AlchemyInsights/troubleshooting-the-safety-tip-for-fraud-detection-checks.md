---
title: Felsökning av säkerhetstipset för bedrägeriidentifieringskontroller
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759530"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="cdfc5-102">Felsökning av säkerhetstipset för bedrägeriidentifieringskontroller</span><span class="sxs-lookup"><span data-stu-id="cdfc5-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="cdfc5-103">Om du får ett säkerhetstips som säger "Avsändaren misslyckades våra kontroller bedrägeri upptäckt och kanske inte vem de verkar vara", då avsändaren misslyckades med att passera antingen DKIM eller SPF autentisering kontroller.</span><span class="sxs-lookup"><span data-stu-id="cdfc5-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="cdfc5-104">Den bästa metoden för att lösa detta är att avsändaren auktoriserar sig själva.</span><span class="sxs-lookup"><span data-stu-id="cdfc5-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="cdfc5-105">Om avsändaren skickar för din räkning måste du auktorisera dem genom att lägga till avsändarens IP-adress i din SPF-post.</span><span class="sxs-lookup"><span data-stu-id="cdfc5-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="cdfc5-106">Mer information [finns i Felsökning av det röda (misstänkta) säkerhetstipset för kontroller av bedrägeriidentifiering.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)</span><span class="sxs-lookup"><span data-stu-id="cdfc5-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="cdfc5-107">Här är några andra länkar som kan hjälpa:</span><span class="sxs-lookup"><span data-stu-id="cdfc5-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="cdfc5-108">Så här använder Microsoft avsändande principramverk (SPF) för att förhindra förfalskning</span><span class="sxs-lookup"><span data-stu-id="cdfc5-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="cdfc5-109">Konfigurera SPF för att förhindra förfalskning</span><span class="sxs-lookup"><span data-stu-id="cdfc5-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
