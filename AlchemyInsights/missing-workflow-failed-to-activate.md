---
title: Arbetsflödet som saknas kunde inte aktiveras
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052631"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="dabc9-102">Arbetsflödet som saknas kunde inte aktiveras</span><span class="sxs-lookup"><span data-stu-id="dabc9-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="dabc9-103">I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbetsflöde (till exempel "godkännande-SharePoint 2010") i en lista eller ett bibliotek.</span><span class="sxs-lookup"><span data-stu-id="dabc9-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="dabc9-104">Lös problemet så här:</span><span class="sxs-lookup"><span data-stu-id="dabc9-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="dabc9-105">Öppna rotwebbplatsen för webbplatssamlingen i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="dabc9-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="dabc9-106">Under **platsobjekt**väljer du **arbetsflöden**.</span><span class="sxs-lookup"><span data-stu-id="dabc9-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="dabc9-107">I det **nya** avsnittet i menyfliksområdet för **arbetsflöden** väljer du **återanvändbart arbetsflöde**.</span><span class="sxs-lookup"><span data-stu-id="dabc9-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="dabc9-108">I formuläret **skapa återanvändbart arbetsflöde** anger du namnet \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="dabc9-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="dabc9-109">För **plattformstyp**klickar du på **SharePoint 2010 Workflow**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="dabc9-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="dabc9-110">Välj **publicera**i avsnittet **Spara** i menyfliksområdet för **arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="dabc9-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="dabc9-111">Välj **publicera globalt**i avsnittet **Hantera** i menyfliksområdet för **arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="dabc9-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="dabc9-112">I bekräftelsedialogrutan som visas väljer du **OK**.</span><span class="sxs-lookup"><span data-stu-id="dabc9-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="dabc9-113">Leta reda på webbplatssamlingens rotwebbplats i en webbläsare och öppna sedan webbplats **samlingens funktioner**för webbplats **Inställningar** \> .</span><span class="sxs-lookup"><span data-stu-id="dabc9-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="dabc9-114">Växla sedan funktionen **arbetsflöden** :</span><span class="sxs-lookup"><span data-stu-id="dabc9-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="dabc9-115">· Om funktionen är *aktiverad* klickar du på **inaktivera** och sedan på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="dabc9-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="dabc9-116">· Om funktionen är *inaktive* rad klickar du på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="dabc9-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="dabc9-117">För mer information hänvisas till följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="dabc9-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

