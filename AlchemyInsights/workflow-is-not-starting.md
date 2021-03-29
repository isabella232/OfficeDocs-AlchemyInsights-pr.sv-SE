---
title: Arbetsflödet startar inte
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403761"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="a051a-102">Arbetsflödet startar inte</span><span class="sxs-lookup"><span data-stu-id="a051a-102">Workflow is not starting</span></span>

- <span data-ttu-id="a051a-103">SharePoint 2010- och SharePoint 2013-arbetsflödena startar inte.</span><span class="sxs-lookup"><span data-stu-id="a051a-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="a051a-104">Om arbetsflödet inte startar kan det finnas ett tillfälligt tjänstproblem där användarna kan uppleva oregelbundna fördröjningar av arbetsflödets förlopp.</span><span class="sxs-lookup"><span data-stu-id="a051a-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="a051a-105">Titta på [instrumentpanelen för](https://admin.microsoft.com/AdminPortal/Home/servicehealth) tjänstens hälsa för att se om din organisation påverkas.</span><span class="sxs-lookup"><span data-stu-id="a051a-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="a051a-106">Om det har gått mer än 24 timmar sedan problemet sågs för första gången ska du logga ett supportmeddelande.</span><span class="sxs-lookup"><span data-stu-id="a051a-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="a051a-107">I många fall arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="a051a-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="a051a-108">Ge oss minst 24 timmar för att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="a051a-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="a051a-109">SharePoint 2010-arbetsflöden fördröjs vid start.</span><span class="sxs-lookup"><span data-stu-id="a051a-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="a051a-110">Detta inträffar om arbetsflödet utlöses i stora batchar.</span><span class="sxs-lookup"><span data-stu-id="a051a-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="a051a-111">(Till exempel när flera objekt läggs till samtidigt).</span><span class="sxs-lookup"><span data-stu-id="a051a-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="a051a-112">Arbetsflöden är inte utformade för att köras i realtid, så en fördröjning beror på designbeteendet.</span><span class="sxs-lookup"><span data-stu-id="a051a-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="a051a-113">Om arbetsflödet är komplext XMOL (Extensible Object Markup Language) kan kompileringen vara långsam.</span><span class="sxs-lookup"><span data-stu-id="a051a-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="a051a-114">Läs [den här](https://support.microsoft.com//kb/3043697) artikeln.</span><span class="sxs-lookup"><span data-stu-id="a051a-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="a051a-115">Du bör förenkla arbetsflödet eller omarbeta det med microsoft SharePoint 2013-arbetsflödesplattformtypen.</span><span class="sxs-lookup"><span data-stu-id="a051a-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="a051a-116">Om arbetsflödeshistoriken har blivit stor kanske du vill rensa objekten eller skapa en ny historiklista.</span><span class="sxs-lookup"><span data-stu-id="a051a-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="a051a-117">Mer information: [Rensa arbetsflödeshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="a051a-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="a051a-118">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="a051a-118">Related topics</span></span>
<span data-ttu-id="a051a-119">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="a051a-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a051a-120">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="a051a-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a051a-121">SharePoint och Flow</span><span class="sxs-lookup"><span data-stu-id="a051a-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
