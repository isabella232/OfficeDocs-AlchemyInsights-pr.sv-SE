---
title: Arbetsflöde för e-post skickas inte
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
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270690"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="4966f-102">Arbetsflöde för e-post skickas inte</span><span class="sxs-lookup"><span data-stu-id="4966f-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="4966f-103">Skickas inte e-post från arbetsflöden för alla användare eller bara vissa användare, eller om du ser felet **e-postmeddelandet inte kan skickas. Kontrollera att e-postmeddelandet har en giltig mottagare**.</span><span class="sxs-lookup"><span data-stu-id="4966f-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="4966f-104">Kontrollera om användaren finns i **Alla** behörigheter gruppen (listan med användarinformation) för webbplatssamlingen.</span><span class="sxs-lookup"><span data-stu-id="4966f-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="4966f-105">Exempel på direkt URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="4966f-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="4966f-106">Om användaren inte finns, kontrollera att användaren har loggat in på sidan.</span><span class="sxs-lookup"><span data-stu-id="4966f-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="4966f-107">Om det är en extern användare kontrollerar du att deras inbjudan har accepterats.</span><span class="sxs-lookup"><span data-stu-id="4966f-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="4966f-108">Om användaren finns i gruppen behörigheter kontrollera e-postadressen är korrekt.</span><span class="sxs-lookup"><span data-stu-id="4966f-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="4966f-109">Om användare e-postadress har angetts här, skapar du aviseringen för användaren vilket tvingar synkronisering av användarkontot från profiler av SharePoint för den här webbplatssamlingen.</span><span class="sxs-lookup"><span data-stu-id="4966f-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="4966f-110">E-post från arbetsflöden skickas till webbplatssamlingens administratörer men inte till andra användare och se felet \*\*http-förbjudet att <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="4966f-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="4966f-111">Se [Åtkomst nekad när du skickat e-brev till grupper](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="4966f-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="4966f-112">Kontrollera också att **begränsad åtkomst användarläge behörighet låsning** webbplatssamling funktionen inte är aktiv.</span><span class="sxs-lookup"><span data-stu-id="4966f-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="4966f-113">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="4966f-113">Related topics</span></span>
<span data-ttu-id="4966f-114">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="4966f-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="4966f-115">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="4966f-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="4966f-116">SharePoint och flöde</span><span class="sxs-lookup"><span data-stu-id="4966f-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


