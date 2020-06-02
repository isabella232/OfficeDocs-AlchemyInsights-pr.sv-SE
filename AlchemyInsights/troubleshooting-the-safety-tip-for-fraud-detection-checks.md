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
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505001"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="aa120-102">Felsökning av säkerhetstipset för bedrägeriidentifieringskontroller</span><span class="sxs-lookup"><span data-stu-id="aa120-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="aa120-103">Om du får ett säkerhetstips som säger "Avsändaren misslyckades våra kontroller bedrägeri upptäckt och kanske inte vem de verkar vara", då avsändaren misslyckades med att passera antingen DKIM eller SPF autentisering kontroller.</span><span class="sxs-lookup"><span data-stu-id="aa120-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="aa120-104">Den bästa metoden för att lösa detta är att avsändaren auktoriserar sig själva.</span><span class="sxs-lookup"><span data-stu-id="aa120-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="aa120-105">Om avsändaren skickar för din räkning måste du auktorisera dem genom att lägga till avsändarens IP-adress i din SPF-post.</span><span class="sxs-lookup"><span data-stu-id="aa120-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="aa120-106">Mer information [finns i Felsökning av det röda (misstänkta) säkerhetstipset för kontroller av bedrägeriidentifiering.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)</span><span class="sxs-lookup"><span data-stu-id="aa120-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="aa120-107">Här är några andra länkar som kan hjälpa:</span><span class="sxs-lookup"><span data-stu-id="aa120-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="aa120-108">Så här använder Microsoft avsändande principramverk (SPF) för att förhindra förfalskning</span><span class="sxs-lookup"><span data-stu-id="aa120-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="aa120-109">Konfigurera SPF för att förhindra förfalskning</span><span class="sxs-lookup"><span data-stu-id="aa120-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
