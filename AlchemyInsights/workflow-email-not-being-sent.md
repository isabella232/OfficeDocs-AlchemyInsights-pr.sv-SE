---
title: Arbetsflödesmeddelande skickas inte
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766151"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="2fc14-102">Arbetsflödesmeddelande skickas inte för en SharePoint-lista eller ett SharePoint-bibliotek</span><span class="sxs-lookup"><span data-stu-id="2fc14-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="2fc14-103">E-post från arbetsflöden skickas inte till alla användare eller bara specifika användare, eller så visas felet **E-postmeddelandet kan inte skickas. Kontrollera att e-postmeddelandet har en giltig mottagare**.</span><span class="sxs-lookup"><span data-stu-id="2fc14-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="2fc14-104">Kontrollera om användaren finns i gruppen **Behörigheter för alla personer** (användarinformationslista) för webbplatssamlingen.</span><span class="sxs-lookup"><span data-stu-id="2fc14-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="2fc14-105">Exempel på direkt webbadress:<tenant>https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0</span><span class="sxs-lookup"><span data-stu-id="2fc14-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="2fc14-106">Om användaren inte finns kontrollerar du att användaren är inloggad på sidan.</span><span class="sxs-lookup"><span data-stu-id="2fc14-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="2fc14-107">Om det är en extern användare kontrollerar du att inbjudan har accepterats.</span><span class="sxs-lookup"><span data-stu-id="2fc14-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="2fc14-108">Om användaren finns i behörighetsgruppen kontrollerar du att e-postadressen är korrekt.</span><span class="sxs-lookup"><span data-stu-id="2fc14-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="2fc14-109">Om användarens e-postadress inte anges här skapar du en exempelavisering för den användaren som tvingar synkroniseringen av användarkontot från Användarprofiler för SharePoint till den här webbplatssamlingen.</span><span class="sxs-lookup"><span data-stu-id="2fc14-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="2fc14-110">E-post från arbetsflöden skickas till administratörerna för webbplatssamlingen men inte till andra användare och visas felet **HTTP Forbidden till <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="2fc14-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="2fc14-111">Se [Åtkomst nekad när du skickar ett e-postmeddelande till en SharePoint-grupp](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="2fc14-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="2fc14-112">Kontrollera också att webbplatsinsamlingsfunktionen för **användarbehörighetslåsningsläge** för begränsad åtkomst inte är aktiv.</span><span class="sxs-lookup"><span data-stu-id="2fc14-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="2fc14-113">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="2fc14-113">Related topics</span></span>
<span data-ttu-id="2fc14-114">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="2fc14-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="2fc14-115">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="2fc14-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2fc14-116">SharePoint och flöde</span><span class="sxs-lookup"><span data-stu-id="2fc14-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


