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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657947"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="066be-102">Konfigurera Endpoint DLP</span><span class="sxs-lookup"><span data-stu-id="066be-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="066be-103">Med Microsoft Endpoint DLP kan du utöka funktionerna för DLP-skydd och övervakning till känslig information på enheter med Windows 10.</span><span class="sxs-lookup"><span data-stu-id="066be-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="066be-104">När enheter har registrerats i Enhetshantering kan du skapa DLP-principer för att upprätthålla skyddsåtgärder för objekt.</span><span class="sxs-lookup"><span data-stu-id="066be-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="066be-105">Aktivitetsutforskaren kan användas för att övervaka aktiviteten för känsliga objekt.</span><span class="sxs-lookup"><span data-stu-id="066be-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="066be-106">Mer information finns i [Registrering av enheter i Enhetshantering](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="066be-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="066be-107">Så här kommer du igång med Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="066be-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="066be-108">Se till att du har rätt SKU/prenumerationslicensiering.</span><span class="sxs-lookup"><span data-stu-id="066be-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="066be-109">Mer information finns i [för SKU/prenumerationslicensiering](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="066be-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="066be-110">Kontrollera vilka behörigheter som krävs för att aktivera Enhetshantering, komma åt registreringssidan eller aktivera/inaktivera enhetsövervakning.</span><span class="sxs-lookup"><span data-stu-id="066be-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="066be-111">Mer information finns i [Behörigheter](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="066be-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="066be-112">Registrera enheter i Enhetshantering genom att följa proceduren för registrering av enheter.</span><span class="sxs-lookup"><span data-stu-id="066be-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="066be-113">Mer information finns i [Registrering av enheter](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="066be-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="066be-114">Skapa DLP-principer för att skydda känsliga objekt.</span><span class="sxs-lookup"><span data-stu-id="066be-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="066be-115">Mer information finns i [principscenarier för Endpoint DLP](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="066be-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="066be-116">Mer information om Microsoft Endpoint DLP finns i [Mer information om dataförlustskydd för slutpunkt (förhandsversion) för Microsoft 365 ](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="066be-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="066be-117">**Viktiga steg för datainsamling, om support krävs:**</span><span class="sxs-lookup"><span data-stu-id="066be-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="066be-118">Hämta [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="066be-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="066be-119">Kör verktyget från cmd-fönstret som administratör:</span><span class="sxs-lookup"><span data-stu-id="066be-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="066be-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="066be-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="066be-121">När du uppmanas **att göra det med Ange antalet minuter för att samla in spårningar:** anger du hur många minuter som behövs för att köra scenariot.</span><span class="sxs-lookup"><span data-stu-id="066be-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="066be-122">Kör scenariot.</span><span class="sxs-lookup"><span data-stu-id="066be-122">Run the scenario.</span></span>

<span data-ttu-id="066be-123">Samla in zip-filens utdata som du vill ge till supportagenten.</span><span class="sxs-lookup"><span data-stu-id="066be-123">Collect the Zip file output to give to the Support agent.</span></span>
