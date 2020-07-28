---
title: Ta bort data och rensa enheter från Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440465"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="5a594-102">Ta bort data och rensa enheter från Intune</span><span class="sxs-lookup"><span data-stu-id="5a594-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="5a594-103">Fjärråtgärderna Enhetsåterställning och Enhetsrensning kan användas för att ta bort företagsdata som hanteras av Intune eller för att utföra en fabriksåterställning och återställa enheten till standardinställningarna.</span><span class="sxs-lookup"><span data-stu-id="5a594-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="5a594-104">Logga in på Microsoft 365 Device Management och gå till **Enheter**  >  **alla enheter**.</span><span class="sxs-lookup"><span data-stu-id="5a594-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="5a594-105">Markera den enhet som du vill rensa.</span><span class="sxs-lookup"><span data-stu-id="5a594-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="5a594-106">Välj den typ av fjärrrensning du vill göra.</span><span class="sxs-lookup"><span data-stu-id="5a594-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="5a594-107">Dra bara bort organisationsinformation, medan fullständiga rensningar återställer enheten till fabriksinställningarna.</span><span class="sxs-lookup"><span data-stu-id="5a594-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="5a594-108">Välj **Ja** för att bekräfta.</span><span class="sxs-lookup"><span data-stu-id="5a594-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="5a594-109">Tills rensningen är klar visas åtgärdsstatusen Enhet som Gå i pension i väntan.</span><span class="sxs-lookup"><span data-stu-id="5a594-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="5a594-110">När åtgärden är klar ser du inte längre den mobila enheten i listan över hanterade enheter.</span><span class="sxs-lookup"><span data-stu-id="5a594-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="5a594-111">**Anm.)** Företagsdata kan inte tas bort från enheter som är anslutna till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5a594-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="5a594-112">Fullständig information om effekten av åtgärderna Gå tillbaka och Rensa, inklusive vad som behålls och vad som tas bort, finns i [Ta bort enheter med hjälp av rensning, dra tillbaka eller manuellt avregistrera enheten](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="5a594-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="5a594-113">Information om hur du raderar alla data från en macOS-enhet finns i [Radera alla data från en macOS-enhet](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="5a594-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>