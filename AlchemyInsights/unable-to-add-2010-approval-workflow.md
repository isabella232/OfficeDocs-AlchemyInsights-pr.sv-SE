---
title: Det går inte att lägga till arbetsflödet för godkännande 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582865"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="38b88-102">Det går inte att lägga till arbetsflödet för godkännande 2010</span><span class="sxs-lookup"><span data-stu-id="38b88-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="38b88-103">I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbetsflöde (till exempel "Godkännande – SharePoint 2010") i en lista eller ett bibliotek.</span><span class="sxs-lookup"><span data-stu-id="38b88-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="38b88-104">Så här löser du problemet:</span><span class="sxs-lookup"><span data-stu-id="38b88-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="38b88-105">Öppna webbplatssamlingens rotwebbplats i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="38b88-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="38b88-106">Under **Webbplatsobjekt**väljer du **Arbetsflöden**.</span><span class="sxs-lookup"><span data-stu-id="38b88-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="38b88-107">I avsnittet **Nytt** i **menyfliksområdet Arbetsflöden** väljer du **Återanvändbart arbetsflöde**.</span><span class="sxs-lookup"><span data-stu-id="38b88-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="38b88-108">Ange namnet \*\* *Repair2010* \*\*i formuläret **Skapa återanvändbart arbetsflöde.**</span><span class="sxs-lookup"><span data-stu-id="38b88-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="38b88-109">För **plattformstyp**klickar du på **SharePoint 2010-arbetsflöde**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="38b88-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="38b88-110">Välj **Publicera** i avsnittet Spara **Publish**i **menyfliksområdet Arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="38b88-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="38b88-111">Välj **Publicera globalt**i avsnittet **Hantera** i menyfliksområdet **Arbetsflöde** .</span><span class="sxs-lookup"><span data-stu-id="38b88-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="38b88-112">Välj **OK**i bekräftelsedialogrutan som visas .</span><span class="sxs-lookup"><span data-stu-id="38b88-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="38b88-113">Leta reda på webbplatssamlingens rotwebbplats i en **Site Settings** webbläsare och sedan öppna \> **webbplatsinställningar.**</span><span class="sxs-lookup"><span data-stu-id="38b88-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="38b88-114">Växla **arbetsflödesfunktionen:**</span><span class="sxs-lookup"><span data-stu-id="38b88-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="38b88-115">· Om funktionen är *Aktiverad* klickar du på **Inaktivera** och sedan på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="38b88-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="38b88-116">· Om funktionen är *Inaktiverad* klickar du på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="38b88-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="38b88-117">Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="38b88-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

