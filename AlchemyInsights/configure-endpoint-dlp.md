---
title: Konfigurera DLP för slutpunkt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556034"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="8c299-102">Konfigurera DLP för slutpunkt</span><span class="sxs-lookup"><span data-stu-id="8c299-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="8c299-103">Med Microsoft Endpoint DLP kan du utöka DLP-skydds- och övervakningsfunktionen till känslig information på Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="8c299-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="8c299-104">När enheter har skapats i enhetshantering kan du skapa DLP-principer för att tillämpa skyddsåtgärder på objekt.</span><span class="sxs-lookup"><span data-stu-id="8c299-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="8c299-105">Aktivitetsutforskaren kan användas för att övervaka aktivitet för känsliga objekt.</span><span class="sxs-lookup"><span data-stu-id="8c299-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="8c299-106">Mer information finns [i Onboarding-enheter i enhetshantering](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="8c299-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="8c299-107">Så här kommer du igång med SlutpunktS-DLP:</span><span class="sxs-lookup"><span data-stu-id="8c299-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="8c299-108">Se till att du har rätt SKU/prenumerationslicensiering.</span><span class="sxs-lookup"><span data-stu-id="8c299-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="8c299-109">Mer information finns i [SKU/prenumerationslicensiering](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="8c299-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="8c299-110">Kontrollera de behörigheter som krävs för att aktivera enhetshantering, komma åt introduktionssidan eller aktivera/inaktivera enhetsövervakning.</span><span class="sxs-lookup"><span data-stu-id="8c299-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="8c299-111">Mer information finns i [Behörigheter](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="8c299-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="8c299-112">Ombord enheter i enhetshantering genom att följa anvisningarna enheter.</span><span class="sxs-lookup"><span data-stu-id="8c299-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="8c299-113">Om du saknar alternativet Förhandsgranskning av enhetsanvisning (förhandsversion) under M365-efterlevnadsinställningar bekräftar du att du har rätt licens och behörigheter som refereras ovan. **Settings**</span><span class="sxs-lookup"><span data-stu-id="8c299-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="8c299-114">Mer information finns i [Onboarding-enheter](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="8c299-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="8c299-115">Skapa DLP-principer för att skydda känsliga objekt.</span><span class="sxs-lookup"><span data-stu-id="8c299-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="8c299-116">Mer information finns i [Principscenarier för slutpunkts-DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="8c299-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="8c299-117">Mer information om Microsoft Endpoint DLP finns [i Lär dig mer om microsoft 365 förhindrande av förlust av slutpunktsdata (förhandsversion).](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)</span><span class="sxs-lookup"><span data-stu-id="8c299-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>