---
title: samma som filnamn är bäst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676551"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="4407e-102">Krävs Alchemy Header H1, H2's fungerar inte.</span><span class="sxs-lookup"><span data-stu-id="4407e-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="4407e-103">Bästa praxis och riktlinjer för Alchemy författande:</span><span class="sxs-lookup"><span data-stu-id="4407e-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="4407e-104">**Kapsla inte Alchemy Insights i mappar**- detta kommer att bryta url-strukturen.</span><span class="sxs-lookup"><span data-stu-id="4407e-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="4407e-105">Vi funderar på att fixa det här.</span><span class="sxs-lookup"><span data-stu-id="4407e-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="4407e-106">Filer i mappen **AlchemyInsights** bör ha gemener filnamn med bindestreck för blanksteg ex.</span><span class="sxs-lookup"><span data-stu-id="4407e-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="4407e-107">***hur-till-aktivera-rättstvist-hold***.</span><span class="sxs-lookup"><span data-stu-id="4407e-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="4407e-108">Inkludera regel-ID: t eller bucket-ID:t från [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) i fältet ms.custom.</span><span class="sxs-lookup"><span data-stu-id="4407e-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="4407e-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="4407e-109">ex.</span></span> <span data-ttu-id="4407e-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="4407e-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="4407e-111">Använd resten av metadata högst upp i den här filen som mall.</span><span class="sxs-lookup"><span data-stu-id="4407e-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="4407e-112">I [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net)navigerar du ned till avsnittet **Kundinsiktstitel:** och använd det som utgångspunkt för din H1-titel för insikten.</span><span class="sxs-lookup"><span data-stu-id="4407e-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="4407e-113">Alchemy Insights måste bara ha en enda H1 på toppen eller de kommer att bryta i produktionen.</span><span class="sxs-lookup"><span data-stu-id="4407e-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="4407e-114">H2s renderar inte antingen så använd **fetstil** eller andra konventioner för att beteckna separata avsnitt.</span><span class="sxs-lookup"><span data-stu-id="4407e-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="4407e-115">Fyll sedan i brödtexten med hjälp av utkastmaterialet i avsnittet Kundinsikter på sidan Alkemiregel</span><span class="sxs-lookup"><span data-stu-id="4407e-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="4407e-116">Punktlistor är bra</span><span class="sxs-lookup"><span data-stu-id="4407e-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="4407e-117">Numrerade listor också</span><span class="sxs-lookup"><span data-stu-id="4407e-117">Numbered lists too</span></span>
    1. <span data-ttu-id="4407e-118">**Fet** och *kursiv* är a-ok</span><span class="sxs-lookup"><span data-stu-id="4407e-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="4407e-119">Länkar bör alltid vara antingen **"länkar till webben"/externa** eller **djuplänkar till gränssnittselement**, inte interna länkar.</span><span class="sxs-lookup"><span data-stu-id="4407e-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="4407e-120">Bilder stöds inte officiellt just nu, men de finns på översikten.</span><span class="sxs-lookup"><span data-stu-id="4407e-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="4407e-121">Och detta är egentligen redan lite för lång.</span><span class="sxs-lookup"><span data-stu-id="4407e-121">And this is really already a bit too long.</span></span> <span data-ttu-id="4407e-122">Bästa praxis är cirka 400 tecken ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="4407e-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="4407e-123">När ditt innehåll är klart drar du det till den levande grenen.</span><span class="sxs-lookup"><span data-stu-id="4407e-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="4407e-124">Gå sedan till [Alchemy Partner-portalen](https://alchemyportal.azurewebsites.net) och ange filnamnet i url-fältet.</span><span class="sxs-lookup"><span data-stu-id="4407e-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 