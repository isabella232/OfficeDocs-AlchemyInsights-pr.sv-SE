---
title: 'Felsöka röst brev låda '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679105"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="2decd-102">Felsöka röst brev låda</span><span class="sxs-lookup"><span data-stu-id="2decd-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="2decd-103">Se till att funktionen upptagen vid upptagen är avsiktlig.</span><span class="sxs-lookup"><span data-stu-id="2decd-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="2decd-104">Om den här funktionen inte behövs för den här användaren:</span><span class="sxs-lookup"><span data-stu-id="2decd-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="2decd-105">Gå till [administrations centret för Teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="2decd-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="2decd-106">På vänster räl navigerar   >  **policyn för röst samtal**  >  **Hantera principer** för **samtals principen**.</span><span class="sxs-lookup"><span data-stu-id="2decd-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="2decd-107">Välj **Hantera användare**.</span><span class="sxs-lookup"><span data-stu-id="2decd-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="2decd-108">Sök efter användare och ändra samtals principen till en som har **upptagen med upptagen när** **du** ringer.</span><span class="sxs-lookup"><span data-stu-id="2decd-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="2decd-109">Klicka på **Använd**.</span><span class="sxs-lookup"><span data-stu-id="2decd-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="2decd-110">Ändringar i policyn kan ta upp till 24 timmar att replikera.</span><span class="sxs-lookup"><span data-stu-id="2decd-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="2decd-111">Mer information om den här funktionen finns i: [upptagen med upptagen är tillgängligt när du är i ett samtal](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="2decd-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
