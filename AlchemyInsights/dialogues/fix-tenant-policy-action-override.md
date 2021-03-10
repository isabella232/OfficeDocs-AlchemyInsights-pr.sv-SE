---
title: Åtgärda klientprincip (åsidosättning av åtgärder)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695692"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="6a0d9-102">Åtgärda klientprincip (åsidosättning av åtgärd)</span><span class="sxs-lookup"><span data-stu-id="6a0d9-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="6a0d9-103">En princip mot skräppost i klientorganisationen påverkade det här meddelandet.</span><span class="sxs-lookup"><span data-stu-id="6a0d9-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="6a0d9-104">Så här granskar du principen:</span><span class="sxs-lookup"><span data-stu-id="6a0d9-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="6a0d9-105">Gå till [Säkerhets- och efterlevnadscenter & Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)och gå sedan **till** Policy för skydd mot  >    >  [skräppost.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="6a0d9-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="6a0d9-106">Kontrollera om principkällan **anger** följande:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="6a0d9-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="6a0d9-107">I så fall kontrollerar **du** inställningarna för den princip som påverkade meddelandet på fliken Anpassad.</span><span class="sxs-lookup"><span data-stu-id="6a0d9-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="6a0d9-108">Det är möjligt att standardinställningarna **som tillämpats** på alla Exchange Online Protection-kunder påverkade meddelandet.</span><span class="sxs-lookup"><span data-stu-id="6a0d9-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="6a0d9-109">Mer information om hur du konfigurerar principer för skräppostfilter finns [i Konfigurera principer för skräppostfilter.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="6a0d9-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
