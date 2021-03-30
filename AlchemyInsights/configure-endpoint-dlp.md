---
title: Konfigurera Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402459"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="bca2c-102">Konfigurera Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="bca2c-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="bca2c-103">Med Microsoft Endpoint DLP kan du utöka funktionerna för DLP-skydd och övervakning till känslig information på enheter med Windows 10.</span><span class="sxs-lookup"><span data-stu-id="bca2c-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="bca2c-104">När enheter har registrerats i Enhetshantering kan du skapa DLP-principer för att upprätthålla skyddsåtgärder för objekt.</span><span class="sxs-lookup"><span data-stu-id="bca2c-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="bca2c-105">Aktivitetsutforskaren kan användas för att övervaka aktiviteten för känsliga objekt.</span><span class="sxs-lookup"><span data-stu-id="bca2c-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="bca2c-106">Mer information finns i [Registrering av enheter i Enhetshantering](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="bca2c-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="bca2c-107">Så här kommer du igång med Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="bca2c-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="bca2c-108">Se till att du har rätt SKU/prenumerationslicensiering.</span><span class="sxs-lookup"><span data-stu-id="bca2c-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="bca2c-109">Mer information finns i [för SKU/prenumerationslicensiering](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="bca2c-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="bca2c-110">Kontrollera vilka behörigheter som krävs för att aktivera Enhetshantering, komma åt registreringssidan eller aktivera/inaktivera enhetsövervakning.</span><span class="sxs-lookup"><span data-stu-id="bca2c-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="bca2c-111">Mer information finns i [Behörigheter](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="bca2c-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="bca2c-112">Registrera enheter i Enhetshantering genom att följa proceduren för registrering av enheter.</span><span class="sxs-lookup"><span data-stu-id="bca2c-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="bca2c-113">Om du saknar alternativet för enhetsregistrering (förhandsversion) under **Inställningar** för Microsoft 365 Efterlevnad, bekräftar du att du har rätt licens och behörigheter som nämns ovan.</span><span class="sxs-lookup"><span data-stu-id="bca2c-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="bca2c-114">Mer information finns i [Registrering av enheter](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="bca2c-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="bca2c-115">Skapa DLP-principer för att skydda känsliga objekt.</span><span class="sxs-lookup"><span data-stu-id="bca2c-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="bca2c-116">Mer information finns i [principscenarier för Endpoint DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="bca2c-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="bca2c-117">Mer information om Microsoft Endpoint DLP finns i [Mer information om dataförlustskydd för slutpunkt (förhandsversion) för Microsoft 365 ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="bca2c-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="bca2c-118">**Viktiga steg för datainsamling, om support krävs:**</span><span class="sxs-lookup"><span data-stu-id="bca2c-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="bca2c-119">Ladda ned förhandsversionen av MDATP-klientanalysprogrammet från [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="bca2c-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="bca2c-120">Kör verktyget från cmd-fönstret som administratör:</span><span class="sxs-lookup"><span data-stu-id="bca2c-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="bca2c-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="bca2c-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="bca2c-122">Ange det antal minuter som krävs för att köra scenariot när du uppmanas att göra det med "Ange antalet minuter för att samla in spårningar: "</span><span class="sxs-lookup"><span data-stu-id="bca2c-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="bca2c-123">Kör scenariot</span><span class="sxs-lookup"><span data-stu-id="bca2c-123">Run the scenario</span></span>

<span data-ttu-id="bca2c-124">Ta emot zip-filen som ska ges till supportagenten.</span><span class="sxs-lookup"><span data-stu-id="bca2c-124">Collect the Zip file output to be given to the Support agent.</span></span>
