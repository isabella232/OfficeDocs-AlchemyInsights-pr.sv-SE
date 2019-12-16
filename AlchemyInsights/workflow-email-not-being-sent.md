---
title: Arbetsflödes e-post skickas inte
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049391"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="79304-102">Arbetsflödes e-post skickas inte för en SharePoint-lista eller bibliotek</span><span class="sxs-lookup"><span data-stu-id="79304-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="79304-103">E-post från arbetsflöden skickas inte till alla användare eller endast till vissa användare, eller så visas felmeddelandet **det går inte att skicka e-postmeddelandet. Kontrollera att e-postmeddelandet har en giltig mottagare**.</span><span class="sxs-lookup"><span data-stu-id="79304-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="79304-104">Kontrollera om användaren finns i gruppen **alla personer** behörigheter (användarinformation lista) för webbplatssamlingen.</span><span class="sxs-lookup"><span data-stu-id="79304-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="79304-105">Exempel på direkt URL:<tenant>https://.<sitename>SharePoint.com/Sites//_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="79304-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="79304-106">Om användaren inte finns kontrollerar du att användaren är inloggad på sidan.</span><span class="sxs-lookup"><span data-stu-id="79304-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="79304-107">Om det är en extern användare, se till att deras inbjudan har accepterats.</span><span class="sxs-lookup"><span data-stu-id="79304-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="79304-108">Om användaren finns i gruppen behörigheter, kontrollera att e-postadressen är korrekt.</span><span class="sxs-lookup"><span data-stu-id="79304-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="79304-109">Om användarnas e-postadress inte anges här, skapa en exempel avisering för användaren som tvingar synkronisering av användarkontot från användarprofiler i SharePoint till den här webbplatssamlingen.</span><span class="sxs-lookup"><span data-stu-id="79304-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="79304-110">E-post från arbetsflöden skickas till administratörer för webbplatssamlingen, men inte till andra användare och se felet **http förbjuden till <span>https:</span>//url/_vti_bin/client.XVC.sp.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="79304-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="79304-111">Se [åtkomst nekad när du skickar ett e-postmeddelande till en SharePoint-grupp](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="79304-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="79304-112">Kontrollera också att den **begränsad åtkomst användare behörighet låsning läge** webbplatssamling funktionen inte är aktiv.</span><span class="sxs-lookup"><span data-stu-id="79304-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="79304-113">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="79304-113">Related topics</span></span>
<span data-ttu-id="79304-114">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="79304-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="79304-115">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="79304-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="79304-116">SharePoint och Flow</span><span class="sxs-lookup"><span data-stu-id="79304-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


