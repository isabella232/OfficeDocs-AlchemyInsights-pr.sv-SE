---
title: Fel när e-post blockeras av SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783821"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="1e5d1-102">Det gick inte att skicka e-post: klient värden blockerades med spamhaus</span><span class="sxs-lookup"><span data-stu-id="1e5d1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="1e5d1-103">Den IP-adress som skickade meddelandet finns i en block lista som ägs av [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="1e5d1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="1e5d1-104">Orsaker till att spamhaus är blockerade är inte säkert att konton, angripna datorer har en offentlig IP-adress och Internet leverantörens principer.</span><span class="sxs-lookup"><span data-stu-id="1e5d1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="1e5d1-105">Möjliga orsaker:</span><span class="sxs-lookup"><span data-stu-id="1e5d1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="1e5d1-106">För blockerade inkommande meddelanden där du styr käll-e-postservern måste du fastställa orsaken och ta bort det från spamhaus webbplats.</span><span class="sxs-lookup"><span data-stu-id="1e5d1-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="1e5d1-107">För blockerade inkommande meddelanden där käll-IP-adressen tillhör någon annan måste adress ägaren ta bort blocket från spamhaus webbplats.</span><span class="sxs-lookup"><span data-stu-id="1e5d1-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="1e5d1-108">Om IP-adressen finns i princip blockeringslistan (PBL) kan ägaren tilldela en annan statisk IP-adress eller ta bort adressen från PBL.</span><span class="sxs-lookup"><span data-stu-id="1e5d1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="1e5d1-109">Om du har blockerat utgående meddelanden från din domän som är ansluten till Microsoft kan du få det här felet om meddelandena cirkuleras via en tredjepartstjänst.</span><span class="sxs-lookup"><span data-stu-id="1e5d1-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="1e5d1-110">Du kan använda ett WHOIS för att hitta den blockerade IP-adressen.</span><span class="sxs-lookup"><span data-stu-id="1e5d1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
