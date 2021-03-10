---
title: Göra webbplatsidentifiering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694556"
---
# <a name="do-site-discovery"></a><span data-ttu-id="0daae-102">Göra webbplatsidentifiering</span><span class="sxs-lookup"><span data-stu-id="0daae-102">Do site discovery</span></span>

<span data-ttu-id="0daae-103">Om din organisation fortfarande använder äldre webbprogram och planerar att använda Internet Explorer-läge (vilket de flesta kunder gör) bör du göra ytterligare webbplatsidentifiering.</span><span class="sxs-lookup"><span data-stu-id="0daae-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="0daae-104">**Du har redan distribuerat en äldre version av Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="0daae-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="0daae-105">Om du redan har konfigurerat din företagswebbplatslista så att den fungerar för den äldre versionen av Microsoft Edge är webbplatsidentifieringen nästan klar.</span><span class="sxs-lookup"><span data-stu-id="0daae-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="0daae-106">Det enda du kan behöva göra är att lägga till neutrala webbplatser.</span><span class="sxs-lookup"><span data-stu-id="0daae-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="0daae-107">Neutrala webbplatser är vanligtvis webbplatser som tillhandahåller enkel inloggning (SSO).</span><span class="sxs-lookup"><span data-stu-id="0daae-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="0daae-108">Om du går till en neutral webbplats från Microsoft Edge vill du vara kvar i Microsoft Edge för att autentisera.</span><span class="sxs-lookup"><span data-stu-id="0daae-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="0daae-109">Om du går till en neutral webbplats i Internet Explorer-läge vill du fortsätta att autentisera i Internet Explorer-läge.</span><span class="sxs-lookup"><span data-stu-id="0daae-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="0daae-110">Identifiera SSO-webbplatser eller andra neutrala webbplatser som du använder och lägg till dem i din lista över företagswebbplatser.</span><span class="sxs-lookup"><span data-stu-id="0daae-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="0daae-111">**Internet Explorer är din standardwebbläsare**</span><span class="sxs-lookup"><span data-stu-id="0daae-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="0daae-112">Om du bara använder Internet Explorer nu kanske du inte vet vilka webbplatser som har uppgraderat till moderna webbstandarder och vilka som fortfarande kräver Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0daae-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="0daae-113">Du vill söka efter och lägga till webbplatserna i listan över företagswebbplatser så att du endast kan använda Internet Explorer-läget för de webbplatserna.</span><span class="sxs-lookup"><span data-stu-id="0daae-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="0daae-114">[Identifiering av företagswebbplats](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) identifierar webbplatser som kan behöva Internet Explorer-läge.</span><span class="sxs-lookup"><span data-stu-id="0daae-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="0daae-115">Den kan samla in data på datorer med Windows Internet Explorer 8 via Internet Explorer 11 på Windows 10, Windows 8.1 eller Windows 7.</span><span class="sxs-lookup"><span data-stu-id="0daae-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="0daae-116">**Analysera data**</span><span class="sxs-lookup"><span data-stu-id="0daae-116">**Analyze the data**</span></span>

<span data-ttu-id="0daae-117">När du har samlat in webbplatsdata rekommenderar vi följande fyrastegsprocess för att analysera data:</span><span class="sxs-lookup"><span data-stu-id="0daae-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="0daae-118">Sortera data efter domän och sedan efter URL.</span><span class="sxs-lookup"><span data-stu-id="0daae-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="0daae-119">Definiera gränserna för ett program för att konfigurera för Internet Explorer-läge.</span><span class="sxs-lookup"><span data-stu-id="0daae-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="0daae-120">Du vill ta med alla webbplatser och webbkontroller som definierar programmet, men du vill inte ta med extra webbplatser och kontroller.</span><span class="sxs-lookup"><span data-stu-id="0daae-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="0daae-121">Vissa webbplatser kan vara lika enkla som *https://contoso.com/app1* medan andra kan kräva att du definierar flera webbplatser och sidor.</span><span class="sxs-lookup"><span data-stu-id="0daae-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="0daae-122">Testa programmet för att verifiera att det inte fungerar inbyggt.</span><span class="sxs-lookup"><span data-stu-id="0daae-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="0daae-123">Många webbplatser erbjuder modernt innehåll när de identifierar en modern webbläsare och erbjuder endast äldre innehåll när de upptäcker Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="0daae-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="0daae-124">Lägg till programmet i företagswebbplatslistan om det inte går att testa.</span><span class="sxs-lookup"><span data-stu-id="0daae-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="0daae-125">En god metod är att gruppera alla webbplatser som en app består av.</span><span class="sxs-lookup"><span data-stu-id="0daae-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="0daae-126">På så sätt är det enklare att ta bort hela webbplatsen från Internet Explorer-läget när du uppgraderar en app och börja använda en modern webbläsare för appen.</span><span class="sxs-lookup"><span data-stu-id="0daae-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="0daae-127">När du är klar med webbplatsupptäckten och analyserat data är du redo att börja titta på din kanalstrategi.</span><span class="sxs-lookup"><span data-stu-id="0daae-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

