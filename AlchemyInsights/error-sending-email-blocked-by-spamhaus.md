---
title: Skicka e-postmeddelanden blockeras av SpamHaus fel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527160"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="f1a9d-102">Fel vid överföring av e-post: Klientvärd blockeras med hjälp av Spamhaus</span><span class="sxs-lookup"><span data-stu-id="f1a9d-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="f1a9d-103">IP-adressen som meddelandet är på en Blockeringslista som ägs av [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="f1a9d-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="f1a9d-104">Skälen för att blockeras av Spamhaus inkludera avslöjade konton äventyras av datorer som delar en gemensam IP-adress och principer för Internet-leverantör (ISP).</span><span class="sxs-lookup"><span data-stu-id="f1a9d-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="f1a9d-105">Det är möjligt korrigeringar:</span><span class="sxs-lookup"><span data-stu-id="f1a9d-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="f1a9d-106">För blockerade inkommande meddelanden till Office 365 där du kan bestämma källservern för e-post, måste du ta reda på orsaken och ta bort spärren från webbplatsen Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f1a9d-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="f1a9d-107">Blockerade inkommande meddelanden till Office 365 där källans IP-adress hör till någon annan måste adress ägare ta bort spärren från webbplatsen Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f1a9d-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="f1a9d-108">Om IP-adressen är i princip Block lista (PBL), ägaren tilldela en annan statisk IP-adress eller ta bort adressen från PBL.</span><span class="sxs-lookup"><span data-stu-id="f1a9d-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="f1a9d-109">Du kan få felet om meddelanden dirigeras via en 3: e part tjänst för blockerade utgående meddelanden från din domän i Office 365.</span><span class="sxs-lookup"><span data-stu-id="f1a9d-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="f1a9d-110">Du kan använda verktyget en WHOIS-sökning för att hitta den blockerade IP-adress ägaren.</span><span class="sxs-lookup"><span data-stu-id="f1a9d-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
