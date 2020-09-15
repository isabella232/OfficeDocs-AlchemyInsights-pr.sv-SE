---
title: Det gick inte att aktivera arbets flödet
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667104"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="fa545-102">Det gick inte att aktivera arbets flödet</span><span class="sxs-lookup"><span data-stu-id="fa545-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="fa545-103">I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbets flöde (som "godkännande-SharePoint 2010") i en lista eller ett bibliotek.</span><span class="sxs-lookup"><span data-stu-id="fa545-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="fa545-104">Lös problemet genom att följa de här stegen:</span><span class="sxs-lookup"><span data-stu-id="fa545-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="fa545-105">Öppna webbplatsens rot webbplats i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="fa545-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="fa545-106">Välj **arbets flöden**under **webbplats objekt**.</span><span class="sxs-lookup"><span data-stu-id="fa545-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="fa545-107">I det **nya** avsnittet i menyfliksområdet **arbets flöden** väljer du **återanvändbart arbets flöde**.</span><span class="sxs-lookup"><span data-stu-id="fa545-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="fa545-108">Ange namnet \* \* *Repair2010* \* \* i formuläret **skapa åter användnings Bart arbets flöde** .</span><span class="sxs-lookup"><span data-stu-id="fa545-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="fa545-109">För **plattforms typer**klickar du på **SharePoint 2010-arbetsflöde**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="fa545-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="fa545-110">Välj **publicera**i avsnittet **Spara** i **arbets flödets** menyfliksområde.</span><span class="sxs-lookup"><span data-stu-id="fa545-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="fa545-111">I avsnittet **Hantera** i menyfliksområdet **arbets flöde** väljer du **publicera globalt**.</span><span class="sxs-lookup"><span data-stu-id="fa545-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="fa545-112">Välj **OK**i bekräftelse dialog rutan som visas.</span><span class="sxs-lookup"><span data-stu-id="fa545-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="fa545-113">I en webbläsare letar du reda på rot webbplatsen för webbplats samlingen och sedan åtkomst till webbplats **Site Settings** \> **samlings funktioner**för webbplats inställningar.</span><span class="sxs-lookup"><span data-stu-id="fa545-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="fa545-114">Sedan kan du växla mellan **arbets flödes** funktionen:</span><span class="sxs-lookup"><span data-stu-id="fa545-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="fa545-115">· Om funktionen är  *aktive rad*  klickar **du på Inaktivera och sedan** på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="fa545-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="fa545-116">· Om funktionen är  *inaktive rad*  klickar du på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="fa545-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="fa545-117">Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="fa545-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

