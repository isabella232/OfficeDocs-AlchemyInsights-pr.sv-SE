---
title: Utgående e-post till mappen skräp post
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769201"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="71a1a-102">Utgående e-post till mappen skräp post</span><span class="sxs-lookup"><span data-stu-id="71a1a-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="71a1a-103">Om du ser utgående meddelanden som skräp post gör du följande:</span><span class="sxs-lookup"><span data-stu-id="71a1a-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="71a1a-104">Om du inte redan har gjort det bör du överväga att [Konfigurera aviseringar om utgående skräp post](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="71a1a-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="71a1a-105">Använd [meddelande spårning](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) för att se om det utgående meddelandet har den alternativa **Spam** informationen: Använd en pool med **hög risk**.</span><span class="sxs-lookup"><span data-stu-id="71a1a-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="71a1a-106">För dessa meddelanden markerar du meddelandets innehåll för att se vad som kan betraktas som skräp post.</span><span class="sxs-lookup"><span data-stu-id="71a1a-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="71a1a-107">Signaturer kan till exempel orsaka problem för många användare.</span><span class="sxs-lookup"><span data-stu-id="71a1a-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="71a1a-108">Om du har flera exempel på legitima utgående meddelanden som marker ATS som skräp post öppnar du ett support ärende och ber support agenten att skicka in dina meddelanden som falsk positiva till våra spam.</span><span class="sxs-lookup"><span data-stu-id="71a1a-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="71a1a-109">Var beredd på att tillhandahålla exempel meddelanden som innehåller alla meddelandehuvuden.</span><span class="sxs-lookup"><span data-stu-id="71a1a-109">Be prepared to provide sample messages that include all message headers.</span></span>
