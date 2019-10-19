---
title: Arbetsflödet startar inte
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738107"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="cdd84-102">Arbetsflödet startar inte</span><span class="sxs-lookup"><span data-stu-id="cdd84-102">Workflow is not starting</span></span>

- <span data-ttu-id="cdd84-103">SharePoint 2010 och SharePoint 2013 arbetsflöden startar inte.</span><span class="sxs-lookup"><span data-stu-id="cdd84-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="cdd84-104">Om ditt arbetsflöde inte startar kan det finnas ett tillfälligt tjänstproblem där användare kan drabbas av återkommande fördröjningar med arbetsflödes förloppet.</span><span class="sxs-lookup"><span data-stu-id="cdd84-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="cdd84-105">Kontrollera den [service Health instrumentpanelen](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.</span><span class="sxs-lookup"><span data-stu-id="cdd84-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="cdd84-106">Om mer än 24 timmar har gått sedan du först såg detta problem, vänligen logga ett supportärende.</span><span class="sxs-lookup"><span data-stu-id="cdd84-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="cdd84-107">I många fall arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="cdd84-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="cdd84-108">Vänligen ge oss minst 24 timmar för att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="cdd84-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="cdd84-109">SharePoint 2010 arbetsflöden fördröjs på Start.</span><span class="sxs-lookup"><span data-stu-id="cdd84-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="cdd84-110">Detta inträffar om arbetsflödet utlöses i stora partier.</span><span class="sxs-lookup"><span data-stu-id="cdd84-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="cdd84-111">(till exempel när flera objekt läggs till på en gång).</span><span class="sxs-lookup"><span data-stu-id="cdd84-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="cdd84-112">Arbetsflöden är inte utformade för att köras i realtid, så en fördröjning är avsiktligt beteende.</span><span class="sxs-lookup"><span data-stu-id="cdd84-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="cdd84-113">Om arbetsflödet är komplext Extensible Object Markup Language (XMOL), kan kompilering vara långsam.</span><span class="sxs-lookup"><span data-stu-id="cdd84-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="cdd84-114">Kontrollera [den här](https://support.microsoft.com//kb/3043697) artikeln.</span><span class="sxs-lookup"><span data-stu-id="cdd84-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="cdd84-115">Du bör förenkla arbetsflödet eller omforma det med hjälp av Microsoft SharePoint 2013 arbetsflödestypen plattform.</span><span class="sxs-lookup"><span data-stu-id="cdd84-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="cdd84-116">Om arbetsflödeshistoriken har blivit stor kanske du vill rensa objekten eller skapa en ny historiklista.</span><span class="sxs-lookup"><span data-stu-id="cdd84-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="cdd84-117">Mer information: [Rensa arbetsflödeshistoriken](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="cdd84-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="cdd84-118">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="cdd84-118">Related topics</span></span>
<span data-ttu-id="cdd84-119">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="cdd84-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="cdd84-120">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="cdd84-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="cdd84-121">SharePoint och Flow</span><span class="sxs-lookup"><span data-stu-id="cdd84-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


