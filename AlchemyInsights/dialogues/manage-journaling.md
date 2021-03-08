---
title: Hantera journalföring
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526147"
---
# <a name="manage-journaling"></a><span data-ttu-id="2f058-102">Hantera journalföring</span><span class="sxs-lookup"><span data-stu-id="2f058-102">Manage journaling</span></span>

<span data-ttu-id="2f058-103">Journaler kan hjälpa din organisation att svara på juridiska och regelmässiga krav och organisationens efterlevnadskrav genom att registrera inkommande och utgående e-postkommunikation.</span><span class="sxs-lookup"><span data-stu-id="2f058-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="2f058-104">Tänk på följande:</span><span class="sxs-lookup"><span data-stu-id="2f058-104">Keep in mind:</span></span>

* <span data-ttu-id="2f058-105">Du måste ha [behörigheten Organisationshantering](https://go.microsoft.com/fwlink/?linkid=2115259) [och Hantering av](https://go.microsoft.com/fwlink/?linkid=2115469) arkivhandlingar innan du kan hantera journaler.</span><span class="sxs-lookup"><span data-stu-id="2f058-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="2f058-106">Du måste ha en journalpostlåda och (om du vill) en alternativ journalpostlåda konfigurerad.</span><span class="sxs-lookup"><span data-stu-id="2f058-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="2f058-107">Mer information finns i [Konfigurera journaler i Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="2f058-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="2f058-108">I Exchange Online finns det en gräns för antalet journalregler som du kan skapa.</span><span class="sxs-lookup"><span data-stu-id="2f058-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="2f058-109">Mer information finns i [regelbegränsningar för journaler,](https://go.microsoft.com/fwlink/?linkid=2115261)transport och inkorgar.</span><span class="sxs-lookup"><span data-stu-id="2f058-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="2f058-110">Exchange Online har inte stöd för att leverera journalrapporter till en Exchange Online-postlåda.</span><span class="sxs-lookup"><span data-stu-id="2f058-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="2f058-111">Du måste ange e-postadressen till ett lokalt arkiveringssystem eller en arkiveringstjänst från tredje part som journalpostlådan.</span><span class="sxs-lookup"><span data-stu-id="2f058-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
