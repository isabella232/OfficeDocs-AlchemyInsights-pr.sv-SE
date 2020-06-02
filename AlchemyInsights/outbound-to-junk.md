---
title: Utgående e-post till mappen Skräppost
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 869cd3d9fb8e5fce291244e4a39754d074b11358
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511742"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="5548e-102">Utgående e-post till mappen Skräppost</span><span class="sxs-lookup"><span data-stu-id="5548e-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="5548e-103">Om utgående meddelanden visas som skräppost gör du följande:</span><span class="sxs-lookup"><span data-stu-id="5548e-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="5548e-104">Om du inte redan har gjort det kan du [konfigurera meddelanden om utgående skräppost.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)</span><span class="sxs-lookup"><span data-stu-id="5548e-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="5548e-105">Använd [meddelandespårning](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) för att se om det utgående meddelandet har händelsevärdet **Skräppost** med ytterligare information: **Använd högriskleveranspool**.</span><span class="sxs-lookup"><span data-stu-id="5548e-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="5548e-106">För dessa meddelanden, kontrollera meddelandeinnehållet för att se vad som kan betraktas som skräppost.</span><span class="sxs-lookup"><span data-stu-id="5548e-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="5548e-107">Signaturer kan till exempel ibland orsaka problem för många användare.</span><span class="sxs-lookup"><span data-stu-id="5548e-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="5548e-108">Om du har flera exempel på legitima utgående meddelanden som markeras som Skräppost öppnar du en supportbiljett och ber supportagenten att skicka in dina meddelanden som falska positiva resultat till våra spamanalytiker.</span><span class="sxs-lookup"><span data-stu-id="5548e-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="5548e-109">Var beredd på att tillhandahålla exempelmeddelanden som innehåller alla meddelanderubriker.</span><span class="sxs-lookup"><span data-stu-id="5548e-109">Be prepared to provide sample messages that include all message headers.</span></span>
