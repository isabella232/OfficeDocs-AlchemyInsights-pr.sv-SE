---
title: Fel att skicka e-post blockeras av SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714276"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="fb5fc-102">Fel att skicka e-post: Klientvärden blockerad med Spamhaus</span><span class="sxs-lookup"><span data-stu-id="fb5fc-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="fb5fc-103">IP-adressen som skickade meddelandet finns på en blockeringslista som ägs av [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="fb5fc-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="fb5fc-104">Orsaker till att blockeras av Spamhaus är komprometterade konton, komprometterade datorer som delar en offentlig IP-adress och Internet Service Provider-principer (ISP).</span><span class="sxs-lookup"><span data-stu-id="fb5fc-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="fb5fc-105">Möjliga korrigeringar är:</span><span class="sxs-lookup"><span data-stu-id="fb5fc-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="fb5fc-106">För blockerade inkommande meddelanden där du styr källmeddelandeservern måste du fastställa orsaken och ta bort blocket från Spamhaus webbplats.</span><span class="sxs-lookup"><span data-stu-id="fb5fc-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="fb5fc-107">För blockerade inkommande meddelanden där källans IP-adress tillhör någon annan måste adressägaren ta bort blocket från Spamhaus-webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="fb5fc-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="fb5fc-108">Om IP-adressen finns i PBL (Policy Block List) kan ägaren tilldela en annan statisk IP-adress eller ta bort adressen från PBL.</span><span class="sxs-lookup"><span data-stu-id="fb5fc-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="fb5fc-109">För blockerade utgående meddelanden från din domän som är ansluten till Microsoft kan du få det här felet om meddelandena dirigeras via en tjänst från tredje part.</span><span class="sxs-lookup"><span data-stu-id="fb5fc-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="fb5fc-110">Du kan använda ett WHOIS-uppslagsverktyg för att hitta ägaren till den blockerade IP-adressen.</span><span class="sxs-lookup"><span data-stu-id="fb5fc-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
