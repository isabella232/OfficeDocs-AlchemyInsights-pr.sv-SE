---
title: Defender Endpoint– kontrollera sensorstatus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676335"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="af58c-102">Defender Endpoint– kontrollera sensorstatus</span><span class="sxs-lookup"><span data-stu-id="af58c-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="af58c-103">Panelen **Enheter med sensorproblem** finns på instrumentpanelen Säkerhetsåtgärder.</span><span class="sxs-lookup"><span data-stu-id="af58c-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="af58c-104">Den här panelen ger information om den enskilda enhetens möjlighet att tillhandahålla sensordata och kommunicera med Defender för slutpunkt-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="af58c-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="af58c-105">Den rapporterar hur många enheter som kräver uppmärksamhet och hjälper dig att identifiera problematiska enheter och vidta åtgärder för att korrigera kända problem.</span><span class="sxs-lookup"><span data-stu-id="af58c-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="af58c-106">Två statusindikatorer på panelen anger information om antalet enheter som inte rapporterar korrekt till tjänsten:</span><span class="sxs-lookup"><span data-stu-id="af58c-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="af58c-107">**Felkonfigurerad** Enheter som delvis kan rapportera sensordata till Defender för slutpunktstjänsten och kan ha konfigurationsfel som behöver korrigeras.</span><span class="sxs-lookup"><span data-stu-id="af58c-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="af58c-108">**Inaktiv** Enheter som har slutat rapportera till Defender för slutpunktstjänsten i mer än sju dagar den senaste månaden.</span><span class="sxs-lookup"><span data-stu-id="af58c-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="af58c-109">Om du klickar på någon av grupperna dirigeras du till listan Enheter, filtrerad enligt dina val.</span><span class="sxs-lookup"><span data-stu-id="af58c-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="af58c-110">I listan Enheter kan du filtrera hälsostatuslistan efter följande status:</span><span class="sxs-lookup"><span data-stu-id="af58c-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="af58c-111">**Aktiv** Enheter som aktivt rapporterar till Defender för slutpunktstjänsten.</span><span class="sxs-lookup"><span data-stu-id="af58c-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="af58c-112">**Felkonfigurerad** Enheter som delvis kan rapportera sensordata till Defender för slutpunkt-tjänsten men har konfigurationsfel som behöver korrigeras.</span><span class="sxs-lookup"><span data-stu-id="af58c-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="af58c-113">Felkonfigurerade enheter kan ha en eller en kombination av följande problem:</span><span class="sxs-lookup"><span data-stu-id="af58c-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="af58c-114">Inga sensordata – Enheterna har slutat skicka sensordata.</span><span class="sxs-lookup"><span data-stu-id="af58c-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="af58c-115">Begränsade aviseringar kan utlösas från enheten.</span><span class="sxs-lookup"><span data-stu-id="af58c-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="af58c-116">Nedsatt kommunikation – Möjligheten att kommunicera med en enhet är försämrad.</span><span class="sxs-lookup"><span data-stu-id="af58c-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="af58c-117">Det kan hända att det inte fungerar att skicka filer för djupanalys, blockera filer, isolera enheten från nätverket och andra åtgärder som kräver kommunikation med enheten.</span><span class="sxs-lookup"><span data-stu-id="af58c-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="af58c-118">**Inaktiv** Enheter som har stoppat rapporteringen till Defender för Slutpunkt-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="af58c-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="af58c-119">Du kan ladda ned hela listan i CSV-format med hjälp av funktionen Exportera.</span><span class="sxs-lookup"><span data-stu-id="af58c-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="af58c-120">Mer information finns i Kontrollera [sensorhälsa i Microsoft Defender för slutpunkt](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="af58c-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="af58c-121">Mer information om vad som orsakade att en enhet var inaktiv eller felaktigt konfigurerad finns i Åtgärda defekta sensor [i Microsoft Defender för Slutpunkt.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="af58c-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
