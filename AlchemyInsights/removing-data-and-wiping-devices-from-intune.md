---
title: Tar bort data och rensar enheter från Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416331"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="b4db8-102">Tar bort data och rensar enheter från Intune</span><span class="sxs-lookup"><span data-stu-id="b4db8-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="b4db8-103">Fjärråtgärderna Ta enhet ur bruk och Rensa enhet kan användas för att ta bort företagsdata som hanteras av Intune, eller för att utföra en fabriksåterställning och återställa enheten till dess standardinställningar.</span><span class="sxs-lookup"><span data-stu-id="b4db8-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="b4db8-104">Logga in på Microsoft 365 Enhetshantering och fortsätt till **Enheter** > **Alla enheter**.</span><span class="sxs-lookup"><span data-stu-id="b4db8-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="b4db8-105">Välj den enhet du vill rensa.</span><span class="sxs-lookup"><span data-stu-id="b4db8-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="b4db8-106">Välj den typ av fjärrensning du vill göra.</span><span class="sxs-lookup"><span data-stu-id="b4db8-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="b4db8-107">Ta ur bruk tar endast bort organisationsinformation, medan en hel rensning återställer enheten till fabriksinställningarna.</span><span class="sxs-lookup"><span data-stu-id="b4db8-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="b4db8-108">Bekräfta genom att välja **Ja**.</span><span class="sxs-lookup"><span data-stu-id="b4db8-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="b4db8-109">Tills rensningen är klar visas enhetsåtgärdsstatusen som *Ta ur bruk pågående*.</span><span class="sxs-lookup"><span data-stu-id="b4db8-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="b4db8-110">När åtgärden har slutförts visas inte längre den mobila enheten i listan över hanterade enheter.</span><span class="sxs-lookup"><span data-stu-id="b4db8-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="b4db8-111">Företagsdata kan inte tas bort från enheter som är anslutna till Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b4db8-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="b4db8-112">Fullständig information om effekterna av åtgärderna Ta ur bruk och Rensa, inklusive vad som behålls och vad som tas bort, finns i följande dokumentation:</span><span class="sxs-lookup"><span data-stu-id="b4db8-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="b4db8-113">[Ta bort enheter genom att rensa, ta ur bruk eller avregistrera enheten manuellt](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="b4db8-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="b4db8-114">Så här rensar du endast företagsdata från appar som hanteras av Intune</span><span class="sxs-lookup"><span data-stu-id="b4db8-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="b4db8-115">[Radera alla data från macOS-enheter](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="b4db8-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>