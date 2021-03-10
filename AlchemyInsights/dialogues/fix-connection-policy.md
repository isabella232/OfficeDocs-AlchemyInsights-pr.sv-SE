---
title: Åtgärda anslutningsprincipen
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695889"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="1e794-102">Åtgärda anslutningsprincipen</span><span class="sxs-lookup"><span data-stu-id="1e794-102">Fix connection policy</span></span>

<span data-ttu-id="1e794-103">E-postmeddelandet har markerats som säkert och levererats till användarens inkorg eftersom den avsändande IP-adressen har markerats som säker i principen för anslutningsfilter.</span><span class="sxs-lookup"><span data-stu-id="1e794-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="1e794-104">Så här granskar du principen:</span><span class="sxs-lookup"><span data-stu-id="1e794-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="1e794-105">Gå till [Säkerhets- och efterlevnadscenter & Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)och gå **sedan** till Policy för skydd mot  >    >  [skräppost.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="1e794-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="1e794-106">Välj **anslutningsfilterprincipen** på **fliken Anpassad** och välj sedan **Redigera princip.**</span><span class="sxs-lookup"><span data-stu-id="1e794-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="1e794-107">Granska listan **över tillåtna IP-adresser.**</span><span class="sxs-lookup"><span data-stu-id="1e794-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="1e794-108">Se om **listan Över säkra är** aktiverad.</span><span class="sxs-lookup"><span data-stu-id="1e794-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="1e794-109">Microsoft prenumererar på källor från tredje part med betrodda avsändare.</span><span class="sxs-lookup"><span data-stu-id="1e794-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="1e794-110">Om **listan Över** betrodda avsändare har aktiverats markeras inte dessa som skräppost av misstag.</span><span class="sxs-lookup"><span data-stu-id="1e794-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="1e794-111">Jag rekommenderar att du väljer det här alternativet eftersom det minskar antalet falska positiva meddelanden (bra e-postmeddelanden som klassificeras som skräppost) som du får.</span><span class="sxs-lookup"><span data-stu-id="1e794-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
