---
title: Saknas arbetsflödet kunde inte aktiveras
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418451"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="6c89f-102">Saknas arbetsflödet kunde inte aktiveras</span><span class="sxs-lookup"><span data-stu-id="6c89f-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="6c89f-103">Du kan inte lägga till ett globalt återanvändbart arbetsflöde (till exempel ”godkännande - SharePoint 2010”) i en Microsoft SharePoint-webbplatssamling till en lista eller ett bibliotek.</span><span class="sxs-lookup"><span data-stu-id="6c89f-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="6c89f-104">Lös problemet så här:</span><span class="sxs-lookup"><span data-stu-id="6c89f-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="6c89f-105">Öppna webbplatsen för webbplatssamlingen rot i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="6c89f-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="6c89f-106">Välj **arbetsflöden**under **Platsobjekt**.</span><span class="sxs-lookup"><span data-stu-id="6c89f-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="6c89f-107">Välj **Återanvändbart arbetsflöde**i avsnittet **Nytt** i menyfliksområdet för **arbetsflöden** .</span><span class="sxs-lookup"><span data-stu-id="6c89f-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="6c89f-108">Ange namnet på formuläret **Skapa återanvändbart arbetsflöde** \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="6c89f-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="6c89f-109">Klicka på **SharePoint 2010 arbetsflöde**för **Plattformstyp**och klicka på **OK**.</span><span class="sxs-lookup"><span data-stu-id="6c89f-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="6c89f-110">Välj **Publicera**i avsnittet **Spara** i menyfliksområdet för **arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="6c89f-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="6c89f-111">Välj **Publicera globalt**i avsnittet **Hantera** i menyfliksområdet för **arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="6c89f-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="6c89f-112">Välj **OK**i dialogrutan för bekräftelse.</span><span class="sxs-lookup"><span data-stu-id="6c89f-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="6c89f-113">Hitta webbplatssamlingen rot webbplats i en webbläsare och tillgång till **Webbplatsinställningar** \> **Webbplatssamlingens funktioner**.</span><span class="sxs-lookup"><span data-stu-id="6c89f-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="6c89f-114">Växla sedan funktionen **arbetsflöden** :</span><span class="sxs-lookup"><span data-stu-id="6c89f-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="6c89f-115">· Om funktionen är *aktiverad* , klickar du på **inaktivera,** och klicka sedan på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="6c89f-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="6c89f-116">· Om funktionen är *Inaktiverad* kan du klicka på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="6c89f-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="6c89f-117">Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="6c89f-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

