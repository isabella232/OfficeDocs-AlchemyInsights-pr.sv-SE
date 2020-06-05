---
title: Den dagliga e-postgränsen har överskridits. Arbetsflödet är pausat.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580351"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="a7f5a-103">Den dagliga e-postgränsen har överskridits.</span><span class="sxs-lookup"><span data-stu-id="a7f5a-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="a7f5a-104">Arbetsflödet är pausat.</span><span class="sxs-lookup"><span data-stu-id="a7f5a-104">Workflow is suspended.</span></span>

<span data-ttu-id="a7f5a-105">Det här felet kan tas emot i följande scenarier:</span><span class="sxs-lookup"><span data-stu-id="a7f5a-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="a7f5a-106">Du har ett arbetsflöde i SharePoint Online som använder typen SharePoint 2010 eller SharePoint 2013.You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform platform type.</span><span class="sxs-lookup"><span data-stu-id="a7f5a-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="a7f5a-107">Arbetsflödet är konfigurerat för att skicka ett anpassat e-postmeddelande till fler än 200 användare åt gången, fler än 10 000 mottagare per dag eller fler än 30 meddelanden per minut.</span><span class="sxs-lookup"><span data-stu-id="a7f5a-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="a7f5a-108">När du kör arbetsflödet skickas inte e-postmeddelandet och du märker följande:</span><span class="sxs-lookup"><span data-stu-id="a7f5a-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="a7f5a-109">Om du vill ha ett arbetsflöde med typen SharePoint 2013-plattform bläddrar du till sidan **Arbetsflödesstatus.**</span><span class="sxs-lookup"><span data-stu-id="a7f5a-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="a7f5a-110">På sidan Arbetsflödesstatus är den **interna statusen** inställd på **Startad**och informationsbubblan visar **det inte går att skicka till en mottagare**.</span><span class="sxs-lookup"><span data-stu-id="a7f5a-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="a7f5a-111">Du kan lösa problemet genom att konfigurera arbetsflödet så att det skickar e-postmeddelanden utan att [överskrida exchange online-avsändningsgränserna](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="a7f5a-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="a7f5a-112">Använd till exempel en paus i arbetsflödet, skicka e-postmeddelandet till en Microsoft 365-grupp, en distributionsgrupp eller en e-postaktiverad säkerhetsgrupp eller skicka meddelandet till färre än 200 mottagare åt gången.</span><span class="sxs-lookup"><span data-stu-id="a7f5a-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="a7f5a-113">Mer information finns i följande [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="a7f5a-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="a7f5a-114">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="a7f5a-114">Related topics</span></span>
- [<span data-ttu-id="a7f5a-115">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="a7f5a-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a7f5a-116">SharePoint och flöde</span><span class="sxs-lookup"><span data-stu-id="a7f5a-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 