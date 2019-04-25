---
title: Kontrollerar säkerheten felsökningstips för spårning av bedrägerier
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391227"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="76031-102">Kontrollerar säkerheten felsökningstips för spårning av bedrägerier</span><span class="sxs-lookup"><span data-stu-id="76031-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="76031-103">Om du får ett tips om säkerhet som säger ”avsändaren misslyckades våra bedrägeri identifiering kontroller och kanske inte som de verkar vara” sedan avsändaren gick inte att överföra DKIM eller SPF verifieringskontroller.</span><span class="sxs-lookup"><span data-stu-id="76031-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="76031-104">Det bästa sättet att lösa detta är att auktorisera sig avsändaren.</span><span class="sxs-lookup"><span data-stu-id="76031-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="76031-105">Om avsändaren skickar för din räkning, måste du ge dem genom att lägga till avsändarens IP-adress till SPF-post.</span><span class="sxs-lookup"><span data-stu-id="76031-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="76031-106">Mer information finns i [felsökningstips röd (misstänkta) säkerhet för spårning av bedrägerier kontrolleras](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="76031-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="76031-107">Här följer några länkar som kan hjälpa:</span><span class="sxs-lookup"><span data-stu-id="76031-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="76031-108">Hur Office 365 använder avsändaren policy framework (SPF) för att förhindra förfalskningar</span><span class="sxs-lookup"><span data-stu-id="76031-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="76031-109">Konfigurera SPF i Office 365 för att förhindra förfalskning</span><span class="sxs-lookup"><span data-stu-id="76031-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

