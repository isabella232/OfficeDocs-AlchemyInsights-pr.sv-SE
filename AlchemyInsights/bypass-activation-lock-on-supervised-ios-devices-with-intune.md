---
title: Kringgå aktiveringslås på övervakade iOS-enheter med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424211"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="f8822-102">Kringgå aktiveringslås på övervakade iOS-enheter med Intune</span><span class="sxs-lookup"><span data-stu-id="f8822-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="f8822-103">Möjligheten att kringgå aktiveringslåset på iOS-enheter gör det enklare att återställa från scenariot där en användare aktiverar aktiveringslås på en företagsenhet och sedan lämnar företaget.</span><span class="sxs-lookup"><span data-stu-id="f8822-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="f8822-104">Förutsättningar för att kringgå ett aktiveringslås inkluderar:</span><span class="sxs-lookup"><span data-stu-id="f8822-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="f8822-105">En enhet är som är "övervakad".</span><span class="sxs-lookup"><span data-stu-id="f8822-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="f8822-106">Aktiveringslåset har aktiverats med hjälp av iOS-enhetsbegränsningsprincipen i Intune.</span><span class="sxs-lookup"><span data-stu-id="f8822-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="f8822-107">Dessutom, när du kringgår ett aktiveringslås, bör du:</span><span class="sxs-lookup"><span data-stu-id="f8822-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="f8822-108">Fysiskt besitter enheten som torkas.</span><span class="sxs-lookup"><span data-stu-id="f8822-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="f8822-109">Kopiera koden innan du utfärdar rensningen.</span><span class="sxs-lookup"><span data-stu-id="f8822-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="f8822-110">**Obs:** Rensningskoden är inte skiftlägeskänslig, så "-" tecknen krävs inte.</span><span class="sxs-lookup"><span data-stu-id="f8822-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="f8822-111">Mer information finns i [Kringgå aktiveringslås på övervakade iOS-enheter med Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="f8822-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="f8822-112">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="f8822-112">**FAQ**</span></span>

<span data-ttu-id="f8822-113">F: **Jag utfärdade en fjärråtgärd för att ta bort företagsdata från en enhet, och nu har den fastnat i ett väntande tillstånd.**</span><span class="sxs-lookup"><span data-stu-id="f8822-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="f8822-114">S: För att en fjärråtgärd ska kunna slutföras måste den riktade enheten vara online och felfri.</span><span class="sxs-lookup"><span data-stu-id="f8822-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="f8822-115">I följande situationer förblir fjärråtgärden i väntande tillstånd i 30 dagar eller tills enheten bekräftar kommandot när enheten:</span><span class="sxs-lookup"><span data-stu-id="f8822-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="f8822-116">Har ingen anslutning.</span><span class="sxs-lookup"><span data-stu-id="f8822-116">Does not have connectivity.</span></span>
- <span data-ttu-id="f8822-117">Förlorar sin hanteringsstatus med Intune.</span><span class="sxs-lookup"><span data-stu-id="f8822-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="f8822-118">Om du tror att en enhet inte längre checkar in och att den inte tar bort företagsdata väljer du Ta bort.</span><span class="sxs-lookup"><span data-stu-id="f8822-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="f8822-119">Om du tar bort tas enhetsposten bort så att den inte längre visas i Intune-listan över enheter.</span><span class="sxs-lookup"><span data-stu-id="f8822-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="f8822-120">För att enheten ska bli aktiv igen måste användaren registrera enheten igen.</span><span class="sxs-lookup"><span data-stu-id="f8822-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="f8822-121">F: **Varför är vissa fjärråtgärder inte tillgängliga för mig att använda?**</span><span class="sxs-lookup"><span data-stu-id="f8822-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="f8822-122">S: Alla plattformar stöder inte alla fjärrenhetsåtgärder.</span><span class="sxs-lookup"><span data-stu-id="f8822-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="f8822-123">Följande fjärråtgärder är plattformsspecifika.</span><span class="sxs-lookup"><span data-stu-id="f8822-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="f8822-124">Kringgå aktiveringslås (endast iOS)</span><span class="sxs-lookup"><span data-stu-id="f8822-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="f8822-125">Nystart (endast Windows)</span><span class="sxs-lookup"><span data-stu-id="f8822-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="f8822-126">Förlorat läge (endast iOS)</span><span class="sxs-lookup"><span data-stu-id="f8822-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="f8822-127">Hitta enhet (endast iOS)</span><span class="sxs-lookup"><span data-stu-id="f8822-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="f8822-128">Starta om (endast Windows)</span><span class="sxs-lookup"><span data-stu-id="f8822-128">Restart (Windows only)</span></span>

<span data-ttu-id="f8822-129">Mer information om varje åtgärd finns i [Tillgängliga enhetsåtgärder](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="f8822-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>