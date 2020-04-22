---
title: Det gick inte att aktivera arbetsflödet som saknades
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762119"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="a8348-102">Det gick inte att aktivera arbetsflödet som saknades</span><span class="sxs-lookup"><span data-stu-id="a8348-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="a8348-103">I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbetsflöde (till exempel "Godkännande – SharePoint 2010") i en lista eller ett bibliotek.</span><span class="sxs-lookup"><span data-stu-id="a8348-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="a8348-104">Så här löser du problemet:</span><span class="sxs-lookup"><span data-stu-id="a8348-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="a8348-105">Öppna webbplatssamlingens rotwebbplats i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="a8348-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="a8348-106">Under **Webbplatsobjekt**väljer du **Arbetsflöden**.</span><span class="sxs-lookup"><span data-stu-id="a8348-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="a8348-107">I avsnittet **Nytt** i **menyfliksområdet Arbetsflöden** väljer du **Återanvändbart arbetsflöde**.</span><span class="sxs-lookup"><span data-stu-id="a8348-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="a8348-108">Ange namnet \*\* *Repair2010* \*\*i formuläret **Skapa återanvändbart arbetsflöde.**</span><span class="sxs-lookup"><span data-stu-id="a8348-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="a8348-109">För **plattformstyp**klickar du på **SharePoint 2010-arbetsflöde**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="a8348-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="a8348-110">Välj **Publicera** i avsnittet Spara **Publish**i **menyfliksområdet Arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="a8348-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="a8348-111">Välj **Publicera globalt**i avsnittet **Hantera** i menyfliksområdet **Arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="a8348-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="a8348-112">Välj **OK**i bekräftelsedialogrutan som visas .</span><span class="sxs-lookup"><span data-stu-id="a8348-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="a8348-113">Leta reda på webbplatssamlingens rotwebbplats i en webbläsare och sedan öppna \> **webbplatsinställningar.** **Site Collection Features**</span><span class="sxs-lookup"><span data-stu-id="a8348-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="a8348-114">Växla sedan **arbetsflödesfunktionen:**</span><span class="sxs-lookup"><span data-stu-id="a8348-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="a8348-115">· Om funktionen är *Aktiverad* klickar du på **Inaktivera** och sedan på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="a8348-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="a8348-116">· Om funktionen är *Inaktiverad* klickar du på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="a8348-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="a8348-117">Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="a8348-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

