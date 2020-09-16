---
title: E-postmeddelandet skickas inte
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
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749027"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="aa5d7-102">E-postmeddelandet skickas inte för en SharePoint-lista eller ett bibliotek</span><span class="sxs-lookup"><span data-stu-id="aa5d7-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="aa5d7-103">E-post från arbets flöden skickas inte till alla användare eller bara vissa användare, eller så visas fel **meddelandet. kontrol lera att e-postmeddelandet har en giltig mottagare**.</span><span class="sxs-lookup"><span data-stu-id="aa5d7-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="aa5d7-104">Kontrol lera om användaren finns i gruppen **all personal** behörigheter (användar information) för webbplats samlingen.</span><span class="sxs-lookup"><span data-stu-id="aa5d7-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="aa5d7-105">Exempel direkt adress: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="aa5d7-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="aa5d7-106">Om användaren inte finns kontrollerar du att användaren är inloggad på sidan.</span><span class="sxs-lookup"><span data-stu-id="aa5d7-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="aa5d7-107">Om det är en extern användare kontrollerar du att deras inbjudan har accepterats.</span><span class="sxs-lookup"><span data-stu-id="aa5d7-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="aa5d7-108">Om användaren finns i behörighets gruppen kontrollerar du att e-postadressen är korrekt.</span><span class="sxs-lookup"><span data-stu-id="aa5d7-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="aa5d7-109">Om användarnas e-postadress inte är inställt här skapar du ett exempel på en avisering för den användaren som tvingar synkroniseringen av användar kontot från användar profiler i SharePoint till den här webbplats samlingen.</span><span class="sxs-lookup"><span data-stu-id="aa5d7-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="aa5d7-110">E-post från arbets flöden skickas till webbplats samlingens administratörer men inte till andra användare och se **http-felet otillåtet för <span>https:</span>//url/_vti_bin/client.XVC.sp.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="aa5d7-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="aa5d7-111">Se [åtkomst nekad när du skickar ett e-postmeddelande till en SharePoint-grupp](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="aa5d7-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="aa5d7-112">Kontrol lera också att funktionen för att **nedlåst behörighets läge för användare med begränsad åtkomst** inte är aktiv.</span><span class="sxs-lookup"><span data-stu-id="aa5d7-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="aa5d7-113">Relaterade ämnen</span><span class="sxs-lookup"><span data-stu-id="aa5d7-113">Related topics</span></span>
<span data-ttu-id="aa5d7-114">Vill du prova Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="aa5d7-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="aa5d7-115">Skapa flöde</span><span class="sxs-lookup"><span data-stu-id="aa5d7-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="aa5d7-116">SharePoint och flöde</span><span class="sxs-lookup"><span data-stu-id="aa5d7-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


