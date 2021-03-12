---
title: Åtgärda inställningar för användarprincip/postlåda
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750564"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="cfcb3-102">Åtgärda inställningar för användarprincip/postlåda</span><span class="sxs-lookup"><span data-stu-id="cfcb3-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="cfcb3-103">Skräppostinställningarna på postlådan påverkade det här meddelandet.</span><span class="sxs-lookup"><span data-stu-id="cfcb3-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="cfcb3-104">Gör så här om du vill granska inställningarna:</span><span class="sxs-lookup"><span data-stu-id="cfcb3-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="cfcb3-105">Starta Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="cfcb3-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="cfcb3-106">Mer information finns i [Öppna Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="cfcb3-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="cfcb3-107">Kör det här kommandot (med användarens  **e-postadress): get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="cfcb3-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="cfcb3-108">Kontrollera om avsändarens e-postadress är en del av **TrustedSendersAndDomains** eller **BlockedSendersAndDomains.**</span><span class="sxs-lookup"><span data-stu-id="cfcb3-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="cfcb3-109">Om e-postadressen finns i en av listorna kan du behöva ta bort den.</span><span class="sxs-lookup"><span data-stu-id="cfcb3-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="cfcb3-110">Mer information finns i [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="cfcb3-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
