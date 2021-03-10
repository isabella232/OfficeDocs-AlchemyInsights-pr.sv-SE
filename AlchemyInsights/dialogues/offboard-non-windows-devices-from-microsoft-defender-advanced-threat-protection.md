---
title: Offboard icke-Windows-enheter från Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695161"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="99d1a-102">Offboard icke-Windows-enheter från Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="99d1a-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="99d1a-103">Så här gör du:</span><span class="sxs-lookup"><span data-stu-id="99d1a-103">Here's how:</span></span>

1. <span data-ttu-id="99d1a-104">Följ dokumentationen från tredje part för att koppla bort tredjepartslösningen från Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="99d1a-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="99d1a-105">Ta bort behörigheter för tredjepartslösningen från Azure Active Directory-klienten:</span><span class="sxs-lookup"><span data-stu-id="99d1a-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="99d1a-106">Logga in på [Azure Portal.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="99d1a-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="99d1a-107">Välj **Alla tjänster** Azure Active  >  **Directory** Enterprise  >  **Applications.**</span><span class="sxs-lookup"><span data-stu-id="99d1a-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="99d1a-108">Välj det program du vill använda som offboard.</span><span class="sxs-lookup"><span data-stu-id="99d1a-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="99d1a-109">Välj **Ta bort.**</span><span class="sxs-lookup"><span data-stu-id="99d1a-109">Select **Delete**.</span></span>

<span data-ttu-id="99d1a-110">Mer information finns i [Offboard-enheter som inte är Windows-enheter.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="99d1a-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
