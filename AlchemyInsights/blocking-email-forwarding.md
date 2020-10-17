---
title: 726 blockerar e-postvidarebefordran
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473119"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="7f09e-102">Blockera eller avblockera e-postvidarekoppling</span><span class="sxs-lookup"><span data-stu-id="7f09e-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="7f09e-103">Information om hur du aktiverar och inaktiverar e-postvidarekoppling för en viss post låda finns i [Konfigurera e-postvidarekoppling](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="7f09e-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="7f09e-104">På klient organisations nivå sker kontrollen av extern vidarebefordring med den utgående skräp posten.</span><span class="sxs-lookup"><span data-stu-id="7f09e-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="7f09e-105">Du kan kontrol lera filtrerings principen för utgående e-post från säkerhets-och kompatibilitetstillstånd [här] ( https://protection.office.com/antispam) eller med [kommandot Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="7f09e-105">You can check the outbound spam filter policy from Security and Compliance Center [here] (https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="7f09e-106">Om du får följande fel meddelande: **"550 5.7.520 åtkomst nekad, tillåter din organisation inte extern vidarebefordran"**, kontrol lera att principen är konfigurerad för att aktivera extern automatisk vidarebefordring.</span><span class="sxs-lookup"><span data-stu-id="7f09e-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="7f09e-107">**Obs!** Du rekommenderas att behålla den externa funktionen för utgående e-post som är inaktive rad som standard och aktivera den för användare som behöver extern vidarebefordran genom att skapa en egen princip för dessa användare.</span><span class="sxs-lookup"><span data-stu-id="7f09e-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="7f09e-108">Du kan läsa mer om hur du [konfigurerar extern vidarebefordran av e-post i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="7f09e-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>