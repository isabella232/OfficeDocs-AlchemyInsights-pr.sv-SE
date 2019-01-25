---
title: Saknas arbetsflödet kunde inte aktiveras
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29491829"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="58fe5-102">Saknas arbetsflödet kunde inte aktiveras</span><span class="sxs-lookup"><span data-stu-id="58fe5-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="58fe5-103">Du kan inte lägga till ett globalt återanvändbart arbetsflöde (till exempel ”godkännande - SharePoint 2010”) i en Microsoft SharePoint-webbplatssamling till en lista eller ett bibliotek.</span><span class="sxs-lookup"><span data-stu-id="58fe5-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="58fe5-104">Lös problemet så här:</span><span class="sxs-lookup"><span data-stu-id="58fe5-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="58fe5-105">Öppna webbplatsen för webbplatssamlingen rot i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="58fe5-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="58fe5-106">Välj **arbetsflöden**under **Platsobjekt**.</span><span class="sxs-lookup"><span data-stu-id="58fe5-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="58fe5-107">Välj **Återanvändbart arbetsflöde**i avsnittet **Nytt** i menyfliksområdet för **arbetsflöden** .</span><span class="sxs-lookup"><span data-stu-id="58fe5-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="58fe5-p101">Ange namnet på formuläret **Skapa återanvändbart arbetsflöde** \*\* *Repair2010* \*\*. Klicka på **SharePoint 2010 arbetsflöde**för **Plattformstyp**och klicka på **OK**.</span><span class="sxs-lookup"><span data-stu-id="58fe5-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="58fe5-110">Välj **Publicera**i avsnittet **Spara** i menyfliksområdet för **arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="58fe5-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="58fe5-p102">Välj **Publicera globalt**i avsnittet **Hantera** i menyfliksområdet för **arbetsflöde** . Välj **OK**i dialogrutan för bekräftelse.</span><span class="sxs-lookup"><span data-stu-id="58fe5-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="58fe5-p103">Hitta webbplatssamlingen rot webbplats i en webbläsare och tillgång till **Webbplatsinställningar** \> **Webbplatssamlingens funktioner**. Växla sedan funktionen **arbetsflöden** :</span><span class="sxs-lookup"><span data-stu-id="58fe5-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="58fe5-115">· Om funktionen är *aktiverad* , klickar du på **inaktivera,** och klicka sedan på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="58fe5-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="58fe5-116">· Om funktionen är *Inaktiverad* kan du klicka på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="58fe5-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="58fe5-117">Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="58fe5-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

