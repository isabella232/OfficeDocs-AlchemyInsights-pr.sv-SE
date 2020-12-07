---
title: Vad kan jag göra om Azure-funktionerna inte fungerar korrekt i Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583781"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="58375-102">Vad kan jag göra om Azure-funktionerna inte fungerar korrekt i Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="58375-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="58375-103">Microsoft Edge har [kända problem](https://go.microsoft.com/fwlink/?linkid=2140608) som är relaterade till säkerhets zoner och kan påverka hur Azure-användare loggar in i Windows Admin Center.</span><span class="sxs-lookup"><span data-stu-id="58375-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="58375-104">Om du har problem med att använda Azure-funktioner med Microsoft Edge kan du försöka med följande:</span><span class="sxs-lookup"><span data-stu-id="58375-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="58375-105">Sök efter **Internet-alternativ** på **Start** -menyn och välj det.</span><span class="sxs-lookup"><span data-stu-id="58375-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="58375-106">I dialog rutan **Internet egenskaper** går du till fliken **säkerhet** .</span><span class="sxs-lookup"><span data-stu-id="58375-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="58375-107">Välj zonen **tillförlitliga platser** och välj sedan knappen **stationer** .</span><span class="sxs-lookup"><span data-stu-id="58375-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="58375-108">I dialog rutan **tillförlitliga platser** lägger du till GATEWAYens URL och [https://login.microsoftonline.com](https://login.microsoftonline.com) och och [https://login.live.com](https://login.live.com) väljer sedan **Stäng**.</span><span class="sxs-lookup"><span data-stu-id="58375-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="58375-109">I dialog rutan **Internet egenskaper** går du till fliken **Sekretess** .</span><span class="sxs-lookup"><span data-stu-id="58375-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="58375-110">Välj **Inställningar** i avsnittet **blockering av popup-fönster** .</span><span class="sxs-lookup"><span data-stu-id="58375-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="58375-111">I dialog rutan som öppnas lägger du till gateway-URL: en [https://login.microsoftonline.com](https://login.microsoftonline.com) och och [https://login.live.com](https://login.live.com) väljer sedan **Stäng**.</span><span class="sxs-lookup"><span data-stu-id="58375-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
