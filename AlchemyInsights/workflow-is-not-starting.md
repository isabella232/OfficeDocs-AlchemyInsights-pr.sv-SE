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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738107"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="92712-102">Arbetsflödet startar inte</span><span class="sxs-lookup"><span data-stu-id="92712-102">Workflow is not starting</span></span>

- <span data-ttu-id="92712-103">SharePoint 2010 och SharePoint 2013 arbetsflöden startar inte.</span><span class="sxs-lookup"><span data-stu-id="92712-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="92712-104">Om ditt arbetsflöde inte startar kan det finnas ett tillfälligt tjänstproblem där användare kan drabbas av återkommande fördröjningar med arbetsflödes förloppet.</span><span class="sxs-lookup"><span data-stu-id="92712-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="92712-105">Kontrollera den [service Health instrumentpanelen](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.</span><span class="sxs-lookup"><span data-stu-id="92712-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="92712-106">Om mer än 24 timmar har gått sedan du först såg detta problem, vänligen logga ett supportärende.</span><span class="sxs-lookup"><span data-stu-id="92712-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="92712-107">I många fall arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="92712-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="92712-108">Vänligen ge oss minst 24 timmar för att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="92712-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="92712-109">SharePoint 2010 arbetsflöden fördröjs på Start.</span><span class="sxs-lookup"><span data-stu-id="92712-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="92712-110">Detta inträffar om arbetsflödet utlöses i stora partier.</span><span class="sxs-lookup"><span data-stu-id="92712-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="92712-111">(till exempel när flera objekt läggs till på en gång).</span><span class="sxs-lookup"><span data-stu-id="92712-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="92712-112">Arbetsflöden är inte utformade för att köras i realtid, så en fördröjning är avsiktligt beteende.</span><span class="sxs-lookup"><span data-stu-id="92712-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="92712-113">Om arbetsflödet är komplext Extensible Object Markup Language (XMOL), kan kompilering vara långsam.</span><span class="sxs-lookup"><span data-stu-id="92712-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="92712-114">Kontrollera [den här](https://support.microsoft.com//kb/3043697) artikeln.</span><span class="sxs-lookup"><span data-stu-id="92712-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="92712-115">Du bör förenkla arbetsflödet eller omforma det med hjälp av Microsoft SharePoint 2013 arbetsflödestypen plattform.</span><span class="sxs-lookup"><span data-stu-id="92712-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="92712-116">Om arbetsflödeshistoriken har blivit stor kanske du vill rensa objekten eller skapa en ny historiklista.</span><span class="sxs-lookup"><span data-stu-id="92712-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="92712-117">Mer information: [Rensa arbetsflödeshistoriken](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="92712-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="92712-118">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="92712-118">Related topics</span></span>
<span data-ttu-id="92712-119">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="92712-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="92712-120">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="92712-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="92712-121">SharePoint och Flow</span><span class="sxs-lookup"><span data-stu-id="92712-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


