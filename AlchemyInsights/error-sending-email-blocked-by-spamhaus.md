---
title: Fel när e-post skulle skickas blockerad av SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813742"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="ea8d2-102">Fel när e-post skickas: Klientvärden blockeras med Spamhaus</span><span class="sxs-lookup"><span data-stu-id="ea8d2-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="ea8d2-103">IP-adressen som har skickat meddelandet finns på en blockeringslista som ägs av [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="ea8d2-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="ea8d2-104">Orsaker till att blockeras av Spamhaus är till exempel komprometterade konton, komprometterade datorer som delar en offentlig IP-adress och Internetleverantörens principer.</span><span class="sxs-lookup"><span data-stu-id="ea8d2-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="ea8d2-105">Möjliga korrigeringar är:</span><span class="sxs-lookup"><span data-stu-id="ea8d2-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="ea8d2-106">För blockerade inkommande meddelanden där du styr käll-e-postservern måste du fastställa orsaken och ta bort blockeringen på Spamhaus-webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="ea8d2-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="ea8d2-107">För blockerade inkommande meddelanden där käll-IP-adressen tillhör någon annan måste adressägaren ta bort blockeringen på Spamhaus-webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="ea8d2-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="ea8d2-108">Om IP-adressen finns med på principlistan över blockerade kan ägaren tilldela en annan statisk IP-adress eller ta bort adressen från principlistan över blockerade.</span><span class="sxs-lookup"><span data-stu-id="ea8d2-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="ea8d2-109">För blockerade utgående meddelanden från din domän som är ansluten till Microsoft kan du få det här felet om meddelandena dirigeras via en tredjepartstjänst.</span><span class="sxs-lookup"><span data-stu-id="ea8d2-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="ea8d2-110">Du kan använda WHOIS-sökverktyget för att hitta den blockerade IP-adressägaren.</span><span class="sxs-lookup"><span data-stu-id="ea8d2-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
