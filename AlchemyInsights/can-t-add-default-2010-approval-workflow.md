---
title: Det går inte att lägga till standard 2010 arbetsflöde för godkännande
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29491867"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="b6e3d-102">Det går inte att lägga till standard 2010 arbetsflöde för godkännande</span><span class="sxs-lookup"><span data-stu-id="b6e3d-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="b6e3d-103">Du kan inte lägga till ett globalt återanvändbart arbetsflöde (till exempel ”godkännande - SharePoint 2010”) i en Microsoft SharePoint-webbplatssamling till en lista eller ett bibliotek.</span><span class="sxs-lookup"><span data-stu-id="b6e3d-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="b6e3d-104">Lös problemet så här:</span><span class="sxs-lookup"><span data-stu-id="b6e3d-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="b6e3d-105">Öppna webbplatsen för webbplatssamlingen rot i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="b6e3d-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="b6e3d-106">Välj **arbetsflöden**under **Platsobjekt**.</span><span class="sxs-lookup"><span data-stu-id="b6e3d-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="b6e3d-107">Välj **Återanvändbart arbetsflöde**i avsnittet **Nytt** i menyfliksområdet för **arbetsflöden** .</span><span class="sxs-lookup"><span data-stu-id="b6e3d-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="b6e3d-p101">Ange namnet på formuläret **Skapa återanvändbart arbetsflöde** \* \*\*Repair2010\*\*\*. Välj **Arbetsflöde för SharePoint 2010**för **Plattformstyp**, och välj sedan **OK**.</span><span class="sxs-lookup"><span data-stu-id="b6e3d-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="b6e3d-110">Välj **Publicera**i avsnittet **Spara** i menyfliksområdet för **arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="b6e3d-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="b6e3d-p102">Välj **Publicera globalt**i avsnittet **Hantera** i menyfliksområdet för **arbetsflöde** . Välj **OK**i dialogrutan för bekräftelse.</span><span class="sxs-lookup"><span data-stu-id="b6e3d-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="b6e3d-p103">Hitta webbplatssamlingen rot webbplats i en webbläsare och tillgång till **Webbplatsinställningar** \> **Webbplatssamlingens funktioner**. Växla sedan funktionen **arbetsflöden** :</span><span class="sxs-lookup"><span data-stu-id="b6e3d-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="b6e3d-115">· Om funktionen är *aktiverad* , klickar du på **inaktivera,** och klicka sedan på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="b6e3d-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="b6e3d-116">· Om funktionen är *Inaktiverad* kan du klicka på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="b6e3d-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="b6e3d-117">Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b6e3d-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

