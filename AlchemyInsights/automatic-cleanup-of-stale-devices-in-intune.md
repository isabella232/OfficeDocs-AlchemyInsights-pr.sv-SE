---
title: Automatisk rensning av inaktuella enheter i Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555735"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="a53d3-102">Automatisk rensning av inaktuella enheter i Intune</span><span class="sxs-lookup"><span data-stu-id="a53d3-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="a53d3-103">Intune gör det möjligt för administratören att konfigurera ett tidsintervall mellan 90 och 270 dagar, varefter inaktuella enheter tas bort från tjänsten.</span><span class="sxs-lookup"><span data-stu-id="a53d3-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="a53d3-104">Den här inställningen är organisationsomfattande och när den aktiveras träder i kraft omedelbart.</span><span class="sxs-lookup"><span data-stu-id="a53d3-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="a53d3-105">Alla enheter som inte checkats in på Intune-servern under en period som överskrider inställningen tas bort permanent.</span><span class="sxs-lookup"><span data-stu-id="a53d3-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="a53d3-106">**Anm.)** Endast MDM-enhetsobjekt kan rensas.</span><span class="sxs-lookup"><span data-stu-id="a53d3-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="a53d3-107">EAS endast enhetsobjekt är uteslutna.</span><span class="sxs-lookup"><span data-stu-id="a53d3-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="a53d3-108">För ytterligare information om när en enhet blir berättigad till borttagning baserat på enhetens rensning och dess "tillstånd":</span><span class="sxs-lookup"><span data-stu-id="a53d3-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="a53d3-109">Inställning: **Ta bort enheter efter senaste incheckningsdatum: Ja (något värde (N) i angivna dagar)**</span><span class="sxs-lookup"><span data-stu-id="a53d3-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="a53d3-110">Baserat på värdet (N) som konfigurerats i inställningen tar Intune-tjänsten bort enheten under de angivna dagarna efter att den senast lyckades checka in.</span><span class="sxs-lookup"><span data-stu-id="a53d3-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="a53d3-111">Inställning: **Ta bort enheter efter senaste incheckningsdatum: Nej**</span><span class="sxs-lookup"><span data-stu-id="a53d3-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="a53d3-112">180 dagar efter att enhetscertifikatet har gått ut och inte förnyats tas enheten bort.</span><span class="sxs-lookup"><span data-stu-id="a53d3-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="a53d3-113">**Anm.)** I båda fallen måste enheten registreras i Intune.</span><span class="sxs-lookup"><span data-stu-id="a53d3-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="a53d3-114">Registrering sker under den första enhetsincheckningen med Intune-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="a53d3-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="a53d3-115">Om en enhet registreras framgångsrikt till Intune men inte blir Intune registrerad, tas enheten bort 270 dagar efter registreringen.</span><span class="sxs-lookup"><span data-stu-id="a53d3-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="a53d3-116">(90 dagar för att markera enheten som återkallad och sedan ytterligare 180 dagar för att ta bort posten.)</span><span class="sxs-lookup"><span data-stu-id="a53d3-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="a53d3-117">Det finns för närvarande ingen mekanism i Intune-konsolen för att fastställa utgångsdatumet för enhetscertifieringen för en viss enhet.</span><span class="sxs-lookup"><span data-stu-id="a53d3-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>