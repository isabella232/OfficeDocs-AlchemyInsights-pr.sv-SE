---
title: Problem med att ta bort en offboardad eller inaktiverad enhet från enhetsinventeringen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564610"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="906be-102">Problem med att ta bort en offboardad eller inaktiverad enhet från enhetsinventeringen</span><span class="sxs-lookup"><span data-stu-id="906be-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="906be-103">Microsoft Defender för Slutpunkt tillåter för närvarande inte att enhetsposten för en offboarded eller inaktiv enhet tas bort manuellt från enhetsinventeringen.</span><span class="sxs-lookup"><span data-stu-id="906be-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="906be-104">Av säkerhetsskäl finns enheten kvar i portalen som en historisk post i upp till 180 dagar.</span><span class="sxs-lookup"><span data-stu-id="906be-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="906be-105">Men enhetens data rensas enligt din konfigurerade lagringstid.</span><span class="sxs-lookup"><span data-stu-id="906be-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="906be-106">**Obs!** En offboarded eller inaktiv enhet växlar automatiskt till **inaktivt** läge efter sju dagar.</span><span class="sxs-lookup"><span data-stu-id="906be-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="906be-107">Dessutom räknas inte enheter som inte är aktiva de senaste 30 dagarna in i de data som återspeglar din organisation Hantering av hot och säkerhetsrisker exponeringsresultat eller Microsoft Secure Score för enheter.</span><span class="sxs-lookup"><span data-stu-id="906be-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="906be-108">Om du fortfarande inte vill se vissa enheter i vyn Enhetsinventering kan du prova att placera en enhetstagg för att filtrera bort den inaktiverade enheten från vyn Enhetsinventering.</span><span class="sxs-lookup"><span data-stu-id="906be-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="906be-109">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="906be-109">For more information, see:</span></span>

[<span data-ttu-id="906be-110">Offboard-enheter från Microsoft Defender för Slutpunkt-tjänsten</span><span class="sxs-lookup"><span data-stu-id="906be-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="906be-111">Exponeringsresultat i Hantering av hot och säkerhetsrisker</span><span class="sxs-lookup"><span data-stu-id="906be-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="906be-112">Åtgärda defekta sensorer i Microsoft Defender för Endpoint</span><span class="sxs-lookup"><span data-stu-id="906be-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="906be-113">Så här använder du taggningen effektivt (del 1)</span><span class="sxs-lookup"><span data-stu-id="906be-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="906be-114">Så här använder du taggningen effektivt (del 2)</span><span class="sxs-lookup"><span data-stu-id="906be-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="906be-115">Så här använder du taggningen effektivt (del 3)</span><span class="sxs-lookup"><span data-stu-id="906be-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




