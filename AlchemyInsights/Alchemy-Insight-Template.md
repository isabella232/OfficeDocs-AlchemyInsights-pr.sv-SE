---
title: samma som filnamnet är bäst
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
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800063"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="78e79-102">Obligatoriska Alkemi huvud H1, H2's fungerar inte.</span><span class="sxs-lookup"><span data-stu-id="78e79-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="78e79-103">Metodtips och riktlinjer för redigering av Alkemi:</span><span class="sxs-lookup"><span data-stu-id="78e79-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="78e79-104">**Kapsla inte Alkemi insikter i mappar**- detta bryts url-struktur.</span><span class="sxs-lookup"><span data-stu-id="78e79-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="78e79-105">Vi söker i åtgärda detta.</span><span class="sxs-lookup"><span data-stu-id="78e79-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="78e79-106">Filer i mappen **AlchemyInsights** ska ha gemener filnamn med bindestreck för utrymmen ex.</span><span class="sxs-lookup"><span data-stu-id="78e79-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="78e79-107">***how-till-aktivera-tvist-Håll***.</span><span class="sxs-lookup"><span data-stu-id="78e79-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="78e79-108">Inkludera regel-ID eller bucket-ID från [Alkemi Partner-portalen](https://alchemyportal.azurewebsites.net) i fältet ms.custom.</span><span class="sxs-lookup"><span data-stu-id="78e79-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="78e79-109">fritt.</span><span class="sxs-lookup"><span data-stu-id="78e79-109">ex.</span></span> <span data-ttu-id="78e79-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="78e79-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="78e79-111">Använd resten av metadata överst i den här filen som en mall.</span><span class="sxs-lookup"><span data-stu-id="78e79-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="78e79-112">I [Alkemi-Partner-portalen](https://alchemyportal.azurewebsites.net), gå till avsnittet **kunden Insight titel:** och användning som pekar som en startpunkt för H1-rubriken för insight.</span><span class="sxs-lookup"><span data-stu-id="78e79-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="78e79-113">Alkemi insikter måste ha bara en enda H1 överst eller de bryts i produktionen.</span><span class="sxs-lookup"><span data-stu-id="78e79-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="78e79-114">H2s återge inte så Använd **fetstil** eller andra konventioner att tillkännage separata avsnitt.</span><span class="sxs-lookup"><span data-stu-id="78e79-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="78e79-115">Sedan fyller du i brödtext med utkast material i avsnittet Kund insikter i regel Alkemi-sida</span><span class="sxs-lookup"><span data-stu-id="78e79-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="78e79-116">Punktlistor är bra</span><span class="sxs-lookup"><span data-stu-id="78e79-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="78e79-117">För numrerade listor</span><span class="sxs-lookup"><span data-stu-id="78e79-117">Numbered lists too</span></span>
    1. <span data-ttu-id="78e79-118">**Fet** och *kursiv stil* är a-ok</span><span class="sxs-lookup"><span data-stu-id="78e79-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="78e79-119">Länkar ska alltid vara antingen **”länkar till web” / extern** eller **djup-länkar till gränssnittselement**, inte interna länkar.</span><span class="sxs-lookup"><span data-stu-id="78e79-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="78e79-120">Bilder stöds inte officiellt just nu, men det är på plan.</span><span class="sxs-lookup"><span data-stu-id="78e79-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="78e79-121">Detta är egentligen redan lite för långt.</span><span class="sxs-lookup"><span data-stu-id="78e79-121">And this is really already a bit too long.</span></span> <span data-ttu-id="78e79-122">Bästa praxis är cirka 400 tecken torrsubstanshalt</span><span class="sxs-lookup"><span data-stu-id="78e79-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="78e79-123">När innehållet är klar kan du dra den levande grenen.</span><span class="sxs-lookup"><span data-stu-id="78e79-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="78e79-124">Sedan går du till [Alkemi på partnerportalen](https://alchemyportal.azurewebsites.net) och ange filnamnet i url-fältet.</span><span class="sxs-lookup"><span data-stu-id="78e79-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 