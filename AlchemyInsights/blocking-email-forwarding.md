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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219873"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="572e2-102">Blockera eller avblockera e-postvidarekoppling</span><span class="sxs-lookup"><span data-stu-id="572e2-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="572e2-103">Information om hur du aktiverar och inaktiverar e-postvidarekoppling för en viss post låda finns i [Konfigurera e-postvidarekoppling](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="572e2-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="572e2-104">På klient organisations nivå sker kontrollen av extern vidarebefordring med principen för utgående anti-spam.</span><span class="sxs-lookup"><span data-stu-id="572e2-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="572e2-105">Om den är inaktive rad eller automatisk kan det vara en snabb överföring av e-post med fel meddelandet "550 5.7.520 åtkomst nekad".</span><span class="sxs-lookup"><span data-stu-id="572e2-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="572e2-106">Om vidarebefordran har ställts in på att blockeras är det fel som användarna ser.</span><span class="sxs-lookup"><span data-stu-id="572e2-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="572e2-107">Om vidarebefordran blockeras bör du kontrol lera att den är konfigurerad för att aktivera extern vidarebefordring.</span><span class="sxs-lookup"><span data-stu-id="572e2-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="572e2-108">Du kan kontrol lera filtrerings principen för utgående e-post från säkerhets-och kompatibilitetstillstånd eller genom att köra kommandona GET-HostedOutboundSpamFilterPolicy | fl-namn, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="572e2-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="572e2-109">Om du vill ställa in blockering av autoforwarding visar kommandot samma tillstånd.</span><span class="sxs-lookup"><span data-stu-id="572e2-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="572e2-110">Obs! Du bör behålla den externa autoforwarden inaktive rad i standard filtrerings filtret för utgående e-post och bara aktivera den för användare som behöver extern vidarebefordran genom att skapa en egen princip för dessa användare.</span><span class="sxs-lookup"><span data-stu-id="572e2-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="572e2-111">Du kan läsa mer om hur du [konfigurerar extern vidarebefordran av e-post i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="572e2-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>