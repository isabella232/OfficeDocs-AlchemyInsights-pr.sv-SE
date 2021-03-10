---
title: Åtgärda vanliga problem med Microsoft Defender för Office 365
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
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695629"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="edd93-102">Åtgärda vanliga problem med Microsoft Defender för Office 365</span><span class="sxs-lookup"><span data-stu-id="edd93-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="edd93-103">Här är några lösningar på vanliga problem med Microsoft Defender för Office 365:</span><span class="sxs-lookup"><span data-stu-id="edd93-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="edd93-104">**Meddelandefördröjning:** Om du har problem med att leverans av meddelanden försenas  bör du använda alternativen för dynamisk leverans i principen för säkra bifogade filer.</span><span class="sxs-lookup"><span data-stu-id="edd93-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="edd93-105">Mer information finns i principer [för dynamisk leverans i säkra bifogade filer.](https://go.microsoft.com/fwlink/?linkid=2094106)</span><span class="sxs-lookup"><span data-stu-id="edd93-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="edd93-106">**Rapportera falska positiva eller negativa resultat:** Rapportera meddelandet till Microsoft med hjälp av den här länken: [Microsoft Defender Response Portal.](https://go.microsoft.com/fwlink/?linkid=2092835)</span><span class="sxs-lookup"><span data-stu-id="edd93-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="edd93-107">**Aktivera skydd mot säkra länkar:**</span><span class="sxs-lookup"><span data-stu-id="edd93-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="edd93-108">Logga in på [Säkerhets- och & Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="edd93-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="edd93-109">Gå till **Hothanteringspolicy**  >    >  **– säkra länkar.**</span><span class="sxs-lookup"><span data-stu-id="edd93-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="edd93-110">Öppna **den konfigurerade principen under Principer** som gäller för specifika mottagare.</span><span class="sxs-lookup"><span data-stu-id="edd93-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="edd93-111">Under **Inställningar** väljer du **Använd säkra länkar för meddelanden som skickas inom organisationen.**</span><span class="sxs-lookup"><span data-stu-id="edd93-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
