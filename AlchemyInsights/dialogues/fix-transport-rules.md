---
title: Åtgärda transportregler
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695863"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="87859-102">Åtgärda transportregler</span><span class="sxs-lookup"><span data-stu-id="87859-102">Fix transport rules</span></span>

<span data-ttu-id="87859-103">En anpassad e-postflödesregel påverkade meddelandet.</span><span class="sxs-lookup"><span data-stu-id="87859-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="87859-104">Om du vill granska den exakta regeln gör du följande:</span><span class="sxs-lookup"><span data-stu-id="87859-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="87859-105">Observera **GUID** eller **principnamnet** under Ytterligare information i **resultatet.**</span><span class="sxs-lookup"><span data-stu-id="87859-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="87859-106">Starta Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="87859-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="87859-107">Mer information finns i [Öppna Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="87859-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="87859-108">Kör det här kommandot (med GUID från din inskickning):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="87859-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="87859-109">Granska beskrivningen för att se de konfigurerade villkoren som påverkade meddelandet.</span><span class="sxs-lookup"><span data-stu-id="87859-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="87859-110">Mer information finns i [Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="87859-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
