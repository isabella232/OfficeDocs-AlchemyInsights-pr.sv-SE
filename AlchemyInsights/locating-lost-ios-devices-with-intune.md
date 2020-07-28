---
title: Hitta förlorade iOS-enheter med Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440430"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="59874-102">Hitta förlorade iOS-enheter med Intune</span><span class="sxs-lookup"><span data-stu-id="59874-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="59874-103">Om du aktiverar förlorat läge på en iOS-enhet kan en administratör få ett meddelande och ett kontakttelefonnummer att visas på låsskärmen.</span><span class="sxs-lookup"><span data-stu-id="59874-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="59874-104">När förlorat läge är aktiverat kan administratören använda åtgärden Hitta enhet för att identifiera enhetens fysiska plats.</span><span class="sxs-lookup"><span data-stu-id="59874-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="59874-105">Åtgärden Hitta enhet i Intune fungerar med iOS-enheter för att visa platsen för en viss enhet på en karta.</span><span class="sxs-lookup"><span data-stu-id="59874-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="59874-106">Om du använder den här åtgärden måste iOS-enheten vara i:</span><span class="sxs-lookup"><span data-stu-id="59874-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="59874-107">Övervakat läge</span><span class="sxs-lookup"><span data-stu-id="59874-107">Supervised mode</span></span>
- <span data-ttu-id="59874-108">Förlorat läge</span><span class="sxs-lookup"><span data-stu-id="59874-108">Lost mode</span></span>

<span data-ttu-id="59874-109">Mer information finns i [Aktivera förlorat läge på iOS/iPadOS-enheter med Intune](https://docs.microsoft.com/intune/device-lost-mode) och Hitta förlorade eller stulna [iOS/iPadOS-enheter med Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="59874-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="59874-110">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="59874-110">**FAQ**</span></span>

<span data-ttu-id="59874-111">F: Jag utfärdade en fjärråtgärd för att ta bort företagsdata från en enhet, och nu har den fastnat i ett väntande tillstånd.</span><span class="sxs-lookup"><span data-stu-id="59874-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="59874-112">S: För att en fjärråtgärd ska kunna slutföras måste den riktade enheten vara online och felfri.</span><span class="sxs-lookup"><span data-stu-id="59874-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="59874-113">I följande situationer förblir fjärråtgärden i väntande tillstånd i 30 dagar eller tills enheten bekräftar kommandot:</span><span class="sxs-lookup"><span data-stu-id="59874-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="59874-114">När enheten inte har anslutning</span><span class="sxs-lookup"><span data-stu-id="59874-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="59874-115">När enheten förlorar sin hanteringsstatus med Intune</span><span class="sxs-lookup"><span data-stu-id="59874-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="59874-116">Om du tror att en enhet inte längre checkar in och att den inte kan ta bort företagsdata väljer du Ta bort.</span><span class="sxs-lookup"><span data-stu-id="59874-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="59874-117">Om du tar bort tas enhetsposten bort så att den inte längre visas i Intune-listan över enheter.</span><span class="sxs-lookup"><span data-stu-id="59874-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="59874-118">Om enheten blir aktiv igen måste användaren registrera den igen.</span><span class="sxs-lookup"><span data-stu-id="59874-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="59874-119">F: Varför är vissa fjärråtgärder inte tillgängliga för mig att använda?</span><span class="sxs-lookup"><span data-stu-id="59874-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="59874-120">S: Alla plattformar stöder inte alla fjärrenhetsåtgärder.</span><span class="sxs-lookup"><span data-stu-id="59874-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="59874-121">Följande fjärråtgärder är plattformsspecifika, så de är endast tillgängliga för de noterade plattformarna.</span><span class="sxs-lookup"><span data-stu-id="59874-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="59874-122">Kringgå aktiveringslås (endast iOS)</span><span class="sxs-lookup"><span data-stu-id="59874-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="59874-123">Nystart (endast Windows)</span><span class="sxs-lookup"><span data-stu-id="59874-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="59874-124">Förlorat läge (endast iOS)</span><span class="sxs-lookup"><span data-stu-id="59874-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="59874-125">Hitta enhet (endast iOS)</span><span class="sxs-lookup"><span data-stu-id="59874-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="59874-126">Starta om (endast Windows)</span><span class="sxs-lookup"><span data-stu-id="59874-126">Restart (Windows only)</span></span>

<span data-ttu-id="59874-127">Mer information om varje åtgärd finns i [Tillgängliga enhetsåtgärder](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="59874-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>