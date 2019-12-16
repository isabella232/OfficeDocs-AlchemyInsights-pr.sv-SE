---
title: Arbetsflödet startar inte
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049355"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="caf85-102">Arbetsflödet startar inte</span><span class="sxs-lookup"><span data-stu-id="caf85-102">Workflow is not starting</span></span>

- <span data-ttu-id="caf85-103">SharePoint 2010 och SharePoint 2013 arbetsflöden startar inte.</span><span class="sxs-lookup"><span data-stu-id="caf85-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="caf85-104">Om ditt arbetsflöde inte startar kan det finnas ett tillfälligt tjänstproblem där användare kan drabbas av återkommande fördröjningar med arbetsflödes förloppet.</span><span class="sxs-lookup"><span data-stu-id="caf85-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="caf85-105">Kontrollera den [service Health instrumentpanelen](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.</span><span class="sxs-lookup"><span data-stu-id="caf85-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="caf85-106">Om mer än 24 timmar har gått sedan du först såg detta problem, vänligen logga ett supportärende.</span><span class="sxs-lookup"><span data-stu-id="caf85-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="caf85-107">I många fall arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="caf85-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="caf85-108">Vänligen ge oss minst 24 timmar för att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="caf85-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="caf85-109">SharePoint 2010 arbetsflöden fördröjs på Start.</span><span class="sxs-lookup"><span data-stu-id="caf85-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="caf85-110">Detta inträffar om arbetsflödet utlöses i stora partier.</span><span class="sxs-lookup"><span data-stu-id="caf85-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="caf85-111">(till exempel när flera objekt läggs till på en gång).</span><span class="sxs-lookup"><span data-stu-id="caf85-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="caf85-112">Arbetsflöden är inte utformade för att köras i realtid, så en fördröjning är avsiktligt beteende.</span><span class="sxs-lookup"><span data-stu-id="caf85-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="caf85-113">Om arbetsflödet är komplext Extensible Object Markup Language (XMOL), kan kompilering vara långsam.</span><span class="sxs-lookup"><span data-stu-id="caf85-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="caf85-114">Kontrollera [den här](https://support.microsoft.com//kb/3043697) artikeln.</span><span class="sxs-lookup"><span data-stu-id="caf85-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="caf85-115">Du bör förenkla arbetsflödet eller omforma det med hjälp av Microsoft SharePoint 2013 arbetsflödestypen plattform.</span><span class="sxs-lookup"><span data-stu-id="caf85-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="caf85-116">Om arbetsflödeshistoriken har blivit stor kanske du vill rensa objekten eller skapa en ny historiklista.</span><span class="sxs-lookup"><span data-stu-id="caf85-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="caf85-117">Mer information: [Rensa arbetsflödeshistoriken](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="caf85-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="caf85-118">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="caf85-118">Related topics</span></span>
<span data-ttu-id="caf85-119">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="caf85-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="caf85-120">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="caf85-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="caf85-121">SharePoint och Flow</span><span class="sxs-lookup"><span data-stu-id="caf85-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


