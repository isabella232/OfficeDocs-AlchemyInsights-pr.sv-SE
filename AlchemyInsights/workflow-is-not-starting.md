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
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270798"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="37e08-102">Arbetsflödet startar inte</span><span class="sxs-lookup"><span data-stu-id="37e08-102">Workflow is not starting</span></span>

- <span data-ttu-id="37e08-103">Arbetsflöden för SharePoint 2010 och SharePoint 2013 startar inte.</span><span class="sxs-lookup"><span data-stu-id="37e08-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="37e08-104">Om arbetsflödet inte startar, kan det finnas en tillfällig service problem där användare kan drabbas av återkommande förseningar med arbetsflödet.</span><span class="sxs-lookup"><span data-stu-id="37e08-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="37e08-105">Kontrollera att [Tjänsten hälsa instrumentpanelen](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) för att se om din organisation påverkas.</span><span class="sxs-lookup"><span data-stu-id="37e08-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="37e08-106">Om mer än 24 timmar har gått sedan du först såg problemet, logga en biljett stöd.</span><span class="sxs-lookup"><span data-stu-id="37e08-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="37e08-107">I många fall kan arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="37e08-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="37e08-108">Ge oss minst 24 timmar att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="37e08-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="37e08-109">SharePoint 2010 arbetsflöden fördröjda på start.</span><span class="sxs-lookup"><span data-stu-id="37e08-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="37e08-110">Detta inträffar om arbetsflödet ska utlösas i stora grupper.</span><span class="sxs-lookup"><span data-stu-id="37e08-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="37e08-111">(till exempel när flera artiklar läggs till på en gång).</span><span class="sxs-lookup"><span data-stu-id="37e08-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="37e08-112">Arbetsflöden är inte avsett att köras i realtid, så att en fördröjning är avsiktlig beteende.</span><span class="sxs-lookup"><span data-stu-id="37e08-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="37e08-113">Om arbetsflödet är komplexa Extensible Object Markup Language (XMOL), kan kompilering vara långsam.</span><span class="sxs-lookup"><span data-stu-id="37e08-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="37e08-114">Kontrollera [den här](https://support.microsoft.com/en-us/kb/3043697) artikeln.</span><span class="sxs-lookup"><span data-stu-id="37e08-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="37e08-115">Du bör förenkla arbetsflödet eller modifiera den med hjälp av Microsoft SharePoint 2013 arbetsflöde-plattformstyp.</span><span class="sxs-lookup"><span data-stu-id="37e08-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="37e08-116">Om din arbetsflödeshistorik har blivit stort, kanske du vill rensa objekten eller skapa en ny historiklista.</span><span class="sxs-lookup"><span data-stu-id="37e08-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="37e08-117">Mer Information: [Rensa arbetsflödeshistorik](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="37e08-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="37e08-118">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="37e08-118">Related topics</span></span>
<span data-ttu-id="37e08-119">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="37e08-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="37e08-120">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="37e08-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="37e08-121">SharePoint och flöde</span><span class="sxs-lookup"><span data-stu-id="37e08-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


