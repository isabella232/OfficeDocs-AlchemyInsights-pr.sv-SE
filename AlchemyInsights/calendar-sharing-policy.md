---
title: Kalender delnings princip för 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684248"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="3e00d-102">Princip fel när du delar en kalender</span><span class="sxs-lookup"><span data-stu-id="3e00d-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="3e00d-103">Gör något av följande, efter behov:</span><span class="sxs-lookup"><span data-stu-id="3e00d-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="3e00d-104">Ansluta till Exchange Online med fjärr-PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3e00d-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="3e00d-105">Mer information finns i [ansluta till Exchange Online med fjärr-PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="3e00d-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="3e00d-106">Öppna Exchange Management Shell på den lokala servern.</span><span class="sxs-lookup"><span data-stu-id="3e00d-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="3e00d-107">Ta reda på vilken delnings princip som är tilldelad användaren.</span><span class="sxs-lookup"><span data-stu-id="3e00d-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="3e00d-108">Det gör du genom att köra följande kommando och notera att principen returneras:</span><span class="sxs-lookup"><span data-stu-id="3e00d-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="3e00d-109">Uppdatera delnings principen för användaren.</span><span class="sxs-lookup"><span data-stu-id="3e00d-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="3e00d-110">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="3e00d-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="3e00d-111">Öppna administrationscentret för Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e00d-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="3e00d-112">Klicka på **organisation**och dubbelklicka sedan på den princip som är tilldelad användaren under **individuell delning**.</span><span class="sxs-lookup"><span data-stu-id="3e00d-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="3e00d-113">Det här är den princip som returnerades i steg 2.</span><span class="sxs-lookup"><span data-stu-id="3e00d-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="3e00d-114">På sidan delnings regel väljer du den delnings nivå som du vill tillåta under **Ange vilken information du vill dela**. Klicka på **Spara**.</span><span class="sxs-lookup"><span data-stu-id="3e00d-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="3e00d-115">Mer information finns i: ["principen tillåter inte att behörigheter på den här nivån beviljar åtkomst på denna nivå till en eller flera av mottagarna" när användaren försöker dela kalendern](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="3e00d-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
