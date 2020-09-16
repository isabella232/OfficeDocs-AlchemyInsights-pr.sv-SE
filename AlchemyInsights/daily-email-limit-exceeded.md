---
title: Daglig e-postgräns har överskridits. Arbets flödet är inaktiverat.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731581"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="821ba-103">Daglig e-postgräns har överskridits.</span><span class="sxs-lookup"><span data-stu-id="821ba-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="821ba-104">Arbets flödet är inaktiverat.</span><span class="sxs-lookup"><span data-stu-id="821ba-104">Workflow is suspended.</span></span>

<span data-ttu-id="821ba-105">Det här felet kan tas emot i följande fall:</span><span class="sxs-lookup"><span data-stu-id="821ba-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="821ba-106">Du har ett arbets flöde i SharePoint Online som använder plattforms typen SharePoint 2010 eller SharePoint 2013 Workflow Platform.</span><span class="sxs-lookup"><span data-stu-id="821ba-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="821ba-107">Arbets flödet är konfigurerat för att skicka ett anpassat e-postmeddelande till fler än 200 användare åt gången, mer än 10 000 mottagare per dag eller mer än 30 meddelanden per minut.</span><span class="sxs-lookup"><span data-stu-id="821ba-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="821ba-108">När du kör arbets flödet skickas inte e-postmeddelandet och du märker följande:</span><span class="sxs-lookup"><span data-stu-id="821ba-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="821ba-109">För ett arbets flöde som använder SharePoint 2013-plattforms typen bläddrar du till sidan **arbets flödes status** .</span><span class="sxs-lookup"><span data-stu-id="821ba-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="821ba-110">På sidan arbets flödes status är den **interna statusen** inaktive rad och informations ballongen **visar att** **det inte går att skicka till en mottagare**.</span><span class="sxs-lookup"><span data-stu-id="821ba-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="821ba-111">Undvik det här problemet genom att konfigurera arbets flödet för att skicka e-postmeddelanden utan att överskrida [avsändarenas gränser för Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="821ba-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="821ba-112">Du kan till exempel använda en paus i arbets flödet och skicka e-postmeddelandet till en Microsoft 365-grupp, en distributions grupp eller en e-postaktive rad säkerhets grupp eller skicka meddelandet till färre än 200 mottagare åt gången.</span><span class="sxs-lookup"><span data-stu-id="821ba-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="821ba-113">Mer information finns i följande [artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="821ba-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="821ba-114">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="821ba-114">Related topics</span></span>
- [<span data-ttu-id="821ba-115">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="821ba-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="821ba-116">SharePoint och flöde</span><span class="sxs-lookup"><span data-stu-id="821ba-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 