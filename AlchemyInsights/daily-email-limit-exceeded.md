---
title: Dagliga e-gränsen har överskridits. Arbetsflödet avbryts.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059656"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="ec7a2-103">Dagliga e-gränsen har överskridits.</span><span class="sxs-lookup"><span data-stu-id="ec7a2-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="ec7a2-104">Arbetsflödet avbryts.</span><span class="sxs-lookup"><span data-stu-id="ec7a2-104">Workflow is suspended.</span></span>

<span data-ttu-id="ec7a2-105">Det här felet kan tas emot i följande scenarier:</span><span class="sxs-lookup"><span data-stu-id="ec7a2-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="ec7a2-106">Du har ett arbetsflöde i SharePoint Online som använder SharePoint 2010 eller SharePoint 2013 arbetsflödestypen plattform.</span><span class="sxs-lookup"><span data-stu-id="ec7a2-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="ec7a2-107">Arbetsflödet har konfigurerats för att skicka ett anpassat e-postmeddelande till mer än 200 användare i taget, mer än 10 000 mottagare per dag eller mer än 30 meddelanden per minut.</span><span class="sxs-lookup"><span data-stu-id="ec7a2-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="ec7a2-108">När du kör arbetsflödet skickas inget e-postmeddelandet och följande inträffa:</span><span class="sxs-lookup"><span data-stu-id="ec7a2-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="ec7a2-109">För ett arbetsflöde som använder SharePoint 2013-plattformstyp, bläddra till sidan **Arbetsflödesstatus** .</span><span class="sxs-lookup"><span data-stu-id="ec7a2-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="ec7a2-110">**Interna Status** har värdet **startad**och information pratbubbla visas **Det går inte att skicka till en mottagare**på sidan Arbetsflödesstatus.</span><span class="sxs-lookup"><span data-stu-id="ec7a2-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="ec7a2-111">Undvik det här problemet genom att konfigurera arbetsflödet om du vill skicka e-postmeddelanden utan att överskrida [gränserna för Exchange Online avsändaren](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="ec7a2-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="ec7a2-112">Till exempel använder en paus i arbetsflödet, skicka e-postmeddelandet till en Office 365-grupp, en distributionsgrupp eller grupp med säkerhet aktiverat mail eller skicka meddelandet till färre än 200 mottagare samtidigt.</span><span class="sxs-lookup"><span data-stu-id="ec7a2-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="ec7a2-113">Mer information finns i följande [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="ec7a2-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="ec7a2-114">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="ec7a2-114">Related topics</span></span>
- [<span data-ttu-id="ec7a2-115">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="ec7a2-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ec7a2-116">SharePoint och flöde</span><span class="sxs-lookup"><span data-stu-id="ec7a2-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 