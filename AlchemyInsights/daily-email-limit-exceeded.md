---
title: Daglig email gräns överskridat. Arbetsflödet är avstängt.
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053135"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="0b7f0-103">Daglig email gräns överskridat.</span><span class="sxs-lookup"><span data-stu-id="0b7f0-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="0b7f0-104">Arbetsflödet är avstängt.</span><span class="sxs-lookup"><span data-stu-id="0b7f0-104">Workflow is suspended.</span></span>

<span data-ttu-id="0b7f0-105">Det här felet kan tas emot i följande scenarier:</span><span class="sxs-lookup"><span data-stu-id="0b7f0-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="0b7f0-106">Du har ett arbetsflöde i SharePoint Online som använder den SharePoint 2010 eller SharePoint 2013 arbetsflödestyp plattform.</span><span class="sxs-lookup"><span data-stu-id="0b7f0-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="0b7f0-107">Arbetsflödet har konfigurerats för att skicka ett anpassat e-postmeddelande till mer än 200 användare i taget, mer än 10 000 mottagare per dag eller mer än 30 meddelanden per minut.</span><span class="sxs-lookup"><span data-stu-id="0b7f0-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="0b7f0-108">När du kör arbetsflödet e-postmeddelandet skickas inte och du märker följande beteende:</span><span class="sxs-lookup"><span data-stu-id="0b7f0-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="0b7f0-109">För ett arbetsflöde med plattforms typen SharePoint 2013 bläddrar du till sidan **arbetsflödes status** .</span><span class="sxs-lookup"><span data-stu-id="0b7f0-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="0b7f0-110">På SidanArbetsflödesstatus är **intern status** inställd på **startad**och informationsbubblan **kan inte skickas till en mottagare**.</span><span class="sxs-lookup"><span data-stu-id="0b7f0-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="0b7f0-111">Undvik det här problemet genom att konfigurera arbetsflödet för att skicka e-postmeddelanden utan att överskrida [Exchange Online avsändar gränser](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="0b7f0-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="0b7f0-112">Till exempel använda en paus i arbetsflödet, skicka e-postmeddelandet till en grupp för Office 365, en distributionsgrupp eller e-postaktiverade säkerhetsgruppen eller skicka meddelandet till färre än 200 mottagare i taget.</span><span class="sxs-lookup"><span data-stu-id="0b7f0-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="0b7f0-113">Mer information finns i följande [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="0b7f0-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="0b7f0-114">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="0b7f0-114">Related topics</span></span>
- [<span data-ttu-id="0b7f0-115">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="0b7f0-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="0b7f0-116">SharePoint och Flow</span><span class="sxs-lookup"><span data-stu-id="0b7f0-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 