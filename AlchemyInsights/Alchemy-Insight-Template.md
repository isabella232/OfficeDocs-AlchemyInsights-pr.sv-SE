---
title: samma som fil namnet är bäst
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664152"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="c2015-102">"Obligatoriskt Alchemy-huvud H1, H2's fungerar inte."</span><span class="sxs-lookup"><span data-stu-id="c2015-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="c2015-103">Metod tips och rikt linjer för Alchemy:</span><span class="sxs-lookup"><span data-stu-id="c2015-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="c2015-104">**Kapsla inte in Alchemy insikter i mappar**– Detta raderar URL-strukturen.</span><span class="sxs-lookup"><span data-stu-id="c2015-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="c2015-105">Vi håller på att fixa detta.</span><span class="sxs-lookup"><span data-stu-id="c2015-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="c2015-106">Filer i **AlchemyInsights** -mappen bör ha gemena fil namn med bindestreck.</span><span class="sxs-lookup"><span data-stu-id="c2015-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="c2015-107">***instruktion-handhållning***.</span><span class="sxs-lookup"><span data-stu-id="c2015-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="c2015-108">Inkludera regel-ID eller Bucket-ID från [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net) i fältet MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="c2015-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="c2015-109">hand.</span><span class="sxs-lookup"><span data-stu-id="c2015-109">ex.</span></span> <span data-ttu-id="c2015-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="c2015-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="c2015-111">Använd resten av metadata högst upp i den här filen som mall.</span><span class="sxs-lookup"><span data-stu-id="c2015-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="c2015-112">I [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net)navigerar du ned till avsnittet **kund Insight-rubriken:** och använder den som utgångs punkt för din H1-rubrik för inblicken.</span><span class="sxs-lookup"><span data-stu-id="c2015-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="c2015-113">Alchemy-insikter får bara ha en enda H1 högst upp, eller så kommer de att brytas i produktionen.</span><span class="sxs-lookup"><span data-stu-id="c2015-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="c2015-114">H2S återger vare sig så Använd **fetstil** eller andra konventioner för att ange separata avsnitt.</span><span class="sxs-lookup"><span data-stu-id="c2015-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="c2015-115">Fyll i bröd texten med hjälp av utkastet i avsnittet Customer Insights på Alchemy-regel Sidan</span><span class="sxs-lookup"><span data-stu-id="c2015-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="c2015-116">Det är bra att Visa punkt listor</span><span class="sxs-lookup"><span data-stu-id="c2015-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="c2015-117">Numrerade listor också</span><span class="sxs-lookup"><span data-stu-id="c2015-117">Numbered lists too</span></span>
    1. <span data-ttu-id="c2015-118">**Fetstil** och *kursiv stil* är a-OK</span><span class="sxs-lookup"><span data-stu-id="c2015-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="c2015-119">Länkar ska alltid vara antingen **"länkar till webb"/External** eller **djupa länkar till gränssnitts element**, inte interna länkar.</span><span class="sxs-lookup"><span data-stu-id="c2015-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="c2015-120">Bilder stöds inte för närvarande, men är på översikten.</span><span class="sxs-lookup"><span data-stu-id="c2015-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="c2015-121">Och det är alldeles för långt.</span><span class="sxs-lookup"><span data-stu-id="c2015-121">And this is really already a bit too long.</span></span> <span data-ttu-id="c2015-122">Bästa metod är att 400 tecken---------------------------------</span><span class="sxs-lookup"><span data-stu-id="c2015-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="c2015-123">När innehållet är klart drar du det till den levande grenen.</span><span class="sxs-lookup"><span data-stu-id="c2015-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="c2015-124">Gå sedan till [Alchemy Partner Portal](https://alchemyportal.azurewebsites.net) och ange fil namnet i fältet URL.</span><span class="sxs-lookup"><span data-stu-id="c2015-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 