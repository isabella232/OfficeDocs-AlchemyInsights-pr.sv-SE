---
title: Felsöka säkerhets tips för kontroller för bedrägeri kontroll
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658428"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="508bd-102">Felsöka säkerhets tips för kontroller för bedrägeri kontroll</span><span class="sxs-lookup"><span data-stu-id="508bd-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="508bd-103">Om du får ett säkerhets tips som säger att avsändaren inte kunde kontrol lera bedrägerier och att den inte verkar vara ", kommer avsändaren inte att skicka DKIM eller SPF-verifikations kontroller.</span><span class="sxs-lookup"><span data-stu-id="508bd-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="508bd-104">Den bästa metoden för att lösa det här är att avsändaren auktoriserar sig.</span><span class="sxs-lookup"><span data-stu-id="508bd-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="508bd-105">Om avsändaren skickar åt dig måste du auktorisera den genom att lägga till avsändarens IP-adress i SPF-posten.</span><span class="sxs-lookup"><span data-stu-id="508bd-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="508bd-106">Mer information finns i [Felsöka det röda (misstänkta) säkerhets tipset för bedrägeri kontroll](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="508bd-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="508bd-107">Här är några andra länkar som kan hjälpa dig:</span><span class="sxs-lookup"><span data-stu-id="508bd-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="508bd-108">Hur Microsoft använder avsändarens princip ramverk (SPF) för att förhindra förfalskning</span><span class="sxs-lookup"><span data-stu-id="508bd-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="508bd-109">Konfigurera SPF för att förhindra förfalskning</span><span class="sxs-lookup"><span data-stu-id="508bd-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
