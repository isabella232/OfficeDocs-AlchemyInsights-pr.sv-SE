---
title: 126 Det går inte att hitta ett fel när du får en postlåda i OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426680"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="5dbfb-102">Visas ingen postlåda i Outlook på webben?</span><span class="sxs-lookup"><span data-stu-id="5dbfb-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="5dbfb-103">Om du använder Outlook på webben och  du får en postlåda som inte kunde hittas på grund av felet har det konto som du använde för att ansluta till Outlook på webben inte någon Exchange Online-licens och därför är ingen postlåda kopplad till kontot.</span><span class="sxs-lookup"><span data-stu-id="5dbfb-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="5dbfb-104">Administratören kan tilldela kontot en licens så här:</span><span class="sxs-lookup"><span data-stu-id="5dbfb-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="5dbfb-105">Öppna [administrationscentret för Microsoft 365,](https://portal.office.com/adminportal/home#/homepage) gå  till Aktiva användare **under** avsnittet Användare och välj den användare som ser felet.</span><span class="sxs-lookup"><span data-stu-id="5dbfb-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="5dbfb-106">På den användarsida som öppnas  går du till avsnittet  Licenser och appar, väljer rätt Platsvärde och tilldelar en licens som innehåller Exchange Online (expandera licensen om du vill se dess information).</span><span class="sxs-lookup"><span data-stu-id="5dbfb-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="5dbfb-107">När du är klar klickar du på **Spara ändringar**.</span><span class="sxs-lookup"><span data-stu-id="5dbfb-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="5dbfb-108">I vissa fall, om licensen redan har tilldelats ett användarkonto, kan du lösa problemet och få den korrekt etablerad i systemet genom att ta bort och omtilldela licensen:</span><span class="sxs-lookup"><span data-stu-id="5dbfb-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="5dbfb-109">Kontrollera om dina M365 Exchange Online-prenumerationer (och andra, om du har några) är aktuella och inte nyligen har upphört att gälla.</span><span class="sxs-lookup"><span data-stu-id="5dbfb-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="5dbfb-110">När du har försäkrat dig om att prenumerationen inte har gått ut och en giltig licens har tilldelats användarkontot kan det ta upp till 24 timmar innan licensen etableras, så du kan behöva vänta på att problemet löses.</span><span class="sxs-lookup"><span data-stu-id="5dbfb-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="5dbfb-111">Mer information finns i [Tilldela och hantera licenser.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="5dbfb-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>