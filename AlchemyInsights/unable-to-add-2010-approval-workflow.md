---
title: Det går inte att lägga till arbets flödet för 2010-godkännande
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699753"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="c7876-102">Det går inte att lägga till arbets flödet för 2010-godkännande</span><span class="sxs-lookup"><span data-stu-id="c7876-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="c7876-103">I en Microsoft SharePoint-webbplatssamling kan du inte lägga till ett globalt återanvändbart arbets flöde (som "godkännande-SharePoint 2010") i en lista eller ett bibliotek.</span><span class="sxs-lookup"><span data-stu-id="c7876-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="c7876-104">Lös problemet genom att följa de här stegen:</span><span class="sxs-lookup"><span data-stu-id="c7876-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="c7876-105">Öppna webbplatsens rot webbplats i SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c7876-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="c7876-106">Välj **arbets flöden**under **webbplats objekt**.</span><span class="sxs-lookup"><span data-stu-id="c7876-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="c7876-107">I det **nya** avsnittet i menyfliksområdet **arbets flöden** väljer du **återanvändbart arbets flöde**.</span><span class="sxs-lookup"><span data-stu-id="c7876-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="c7876-108">Ange namnet \* \* *Repair2010* \* \* i formuläret **skapa åter användnings Bart arbets flöde** .</span><span class="sxs-lookup"><span data-stu-id="c7876-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="c7876-109">För **plattforms typer**klickar du på **SharePoint 2010-arbetsflöde**och sedan på **OK**.</span><span class="sxs-lookup"><span data-stu-id="c7876-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="c7876-110">Välj **publicera**i avsnittet **Spara** i **arbets flödets** menyfliksområde.</span><span class="sxs-lookup"><span data-stu-id="c7876-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="c7876-111">I avsnittet **Hantera** i menyfliksområdet **arbets flöde** väljer du **publicera globalt**.</span><span class="sxs-lookup"><span data-stu-id="c7876-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="c7876-112">Välj **OK**i bekräftelse dialog rutan som visas.</span><span class="sxs-lookup"><span data-stu-id="c7876-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="c7876-113">I en webbläsare letar du reda på rot webbplatsen för webbplats samlingen och sedan åtkomst till webbplats **Site Settings** \> **samlings funktioner**för webbplats inställningar.</span><span class="sxs-lookup"><span data-stu-id="c7876-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="c7876-114">Aktivera funktionen **arbets flöden** :</span><span class="sxs-lookup"><span data-stu-id="c7876-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="c7876-115">· Om funktionen är  *aktive rad*  klickar **du på Inaktivera och sedan** på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="c7876-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="c7876-116">· Om funktionen är  *inaktive rad*  klickar du på **Aktivera**.</span><span class="sxs-lookup"><span data-stu-id="c7876-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="c7876-117">Mer information finns i följande [artikel](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c7876-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

