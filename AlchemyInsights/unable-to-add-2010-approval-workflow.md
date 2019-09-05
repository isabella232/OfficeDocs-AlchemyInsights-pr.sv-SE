---
title: Det gick inte att lägga till 2010 Godkännandearbetsflöde
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748702"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="0e0f5-102">Det gick inte att lägga till 2010 Godkännandearbetsflöde</span><span class="sxs-lookup"><span data-stu-id="0e0f5-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="0e0f5-103">I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbetsflöde (till exempel "godkännande-SharePoint 2010") i en lista eller ett bibliotek.</span><span class="sxs-lookup"><span data-stu-id="0e0f5-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0e0f5-104">Lös problemet så här:</span><span class="sxs-lookup"><span data-stu-id="0e0f5-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0e0f5-105">Öppna rotwebbplatsen för webbplatssamlingen i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0e0f5-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0e0f5-106">Under **platsobjekt**väljer du **arbetsflöden**.</span><span class="sxs-lookup"><span data-stu-id="0e0f5-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0e0f5-107">I det **nya** avsnittet i menyfliksområdet för **arbetsflöden** väljer du **återanvändbart arbetsflöde**.</span><span class="sxs-lookup"><span data-stu-id="0e0f5-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0e0f5-108">I formuläret **skapa återanvändbart arbetsflöde** anger du namnet \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="0e0f5-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="0e0f5-109">För **plattformstyp**klickar du på **SharePoint 2010 Workflow**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="0e0f5-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="0e0f5-110">Välj **publicera**i avsnittet **Spara** i menyfliksområdet för **arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="0e0f5-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="0e0f5-111">Välj **publicera globalt**i avsnittet **Hantera** i menyfliksområdet för **arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="0e0f5-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="0e0f5-112">I bekräftelsedialogrutan som visas väljer du **OK**.</span><span class="sxs-lookup"><span data-stu-id="0e0f5-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="0e0f5-113">Leta reda på webbplatssamlingens rotwebbplats i en webbläsare och öppna sedan webbplats **samlingens funktioner**för webbplats **Inställningar** \> .</span><span class="sxs-lookup"><span data-stu-id="0e0f5-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="0e0f5-114">Växla funktionen **arbetsflöden** :</span><span class="sxs-lookup"><span data-stu-id="0e0f5-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0e0f5-115">· Om funktionen är *aktiverad* klickar du på **inaktivera** och sedan på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="0e0f5-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0e0f5-116">· Om funktionen är *inaktive* rad klickar du på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="0e0f5-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0e0f5-117">För mer information hänvisas till följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="0e0f5-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

