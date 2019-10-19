---
title: samma som filnamn är bäst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "35800063"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="d8590-102">Krävs Alchemy header H1, H2's fungerar inte.</span><span class="sxs-lookup"><span data-stu-id="d8590-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="d8590-103">Bästa praxis och riktlinjer för Alchemy författande:</span><span class="sxs-lookup"><span data-stu-id="d8590-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="d8590-104">**Inte kapsla Alchemy insikter i mappar**-detta kommer att bryta URL-strukturen.</span><span class="sxs-lookup"><span data-stu-id="d8590-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="d8590-105">Vi tittar på att fixa detta.</span><span class="sxs-lookup"><span data-stu-id="d8590-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="d8590-106">Filer i mappen **Alchemyinsights** ska ha gemener filnamn med bindestreck för blanksteg ex.</span><span class="sxs-lookup"><span data-stu-id="d8590-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="d8590-107">***hur-till-möjliggöra-rättstvist-Hold***.</span><span class="sxs-lookup"><span data-stu-id="d8590-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="d8590-108">Inkludera regel-ID eller Bucket-ID från [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net) i den MS. Custom fält.</span><span class="sxs-lookup"><span data-stu-id="d8590-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="d8590-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="d8590-109">ex.</span></span> <span data-ttu-id="d8590-110">***MS Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="d8590-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="d8590-111">Använd resten av metadata överst i den här filen som din mall.</span><span class="sxs-lookup"><span data-stu-id="d8590-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="d8590-112">I [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net), Navigera ner till avsnittet **kundinsikt titel:** och använda det som en utgångspunkt för din H1 titel för insikten.</span><span class="sxs-lookup"><span data-stu-id="d8590-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="d8590-113">Alchemy Insights måste ha bara en enda H1 på toppen eller de kommer att bryta i produktionen.</span><span class="sxs-lookup"><span data-stu-id="d8590-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="d8590-114">H2S gör inte heller så Använd **fetstil** eller andra konventioner för att beteckna separata sektioner.</span><span class="sxs-lookup"><span data-stu-id="d8590-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="d8590-115">Fyll sedan i brödtexten med hjälp av utkasts materialet i avsnittet Customer Insights på sidan Alchemy Rule</span><span class="sxs-lookup"><span data-stu-id="d8590-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="d8590-116">Punktlistor är bra</span><span class="sxs-lookup"><span data-stu-id="d8590-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="d8590-117">Numrerade listor för</span><span class="sxs-lookup"><span data-stu-id="d8590-117">Numbered lists too</span></span>
    1. <span data-ttu-id="d8590-118">**Fet** och *kursiv* är a-OK</span><span class="sxs-lookup"><span data-stu-id="d8590-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="d8590-119">Länkar ska alltid vara antingen **"länkar till webb"/externa** eller **djupa länkar till UI element**, inte interna länkar.</span><span class="sxs-lookup"><span data-stu-id="d8590-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="d8590-120">Bilder stöds inte officiellt vid denna tid, men det är på färdplanen.</span><span class="sxs-lookup"><span data-stu-id="d8590-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="d8590-121">Och detta är verkligen redan lite för länge.</span><span class="sxs-lookup"><span data-stu-id="d8590-121">And this is really already a bit too long.</span></span> <span data-ttu-id="d8590-122">Bästa praxis är cirka 400 tecken---------------------------------</span><span class="sxs-lookup"><span data-stu-id="d8590-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="d8590-123">När innehållet är klart drar du det till grenen Live.</span><span class="sxs-lookup"><span data-stu-id="d8590-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="d8590-124">Gå sedan till [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net) och ange filnamnet i URL-fältet.</span><span class="sxs-lookup"><span data-stu-id="d8590-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 