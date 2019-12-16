---
title: Prestandaproblem-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2db0a9442b9fdf1752b654f7c188e641e0a274cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053819"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="cf280-102">SharePoint eller OneDrive är långsam, otillgänglig eller otillgänglig för flera användare</span><span class="sxs-lookup"><span data-stu-id="cf280-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="cf280-103">Om en OneDrive eller SharePoint-webbplats inte är tillgänglig för flera användare som tidigare hade åtkomst, kan det finnas ett tillfälligt problem med tjänsten.</span><span class="sxs-lookup"><span data-stu-id="cf280-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="cf280-104">[Kontrollera den service Health instrumentpanelen](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="cf280-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="cf280-105">**Lägg till och licensiera användaren**</span><span class="sxs-lookup"><span data-stu-id="cf280-105">**Add and license the user**</span></span>

<span data-ttu-id="cf280-106">Se till att du [tilldelar licenser till användare i Office 365 för företag](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="cf280-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="cf280-107">**Tilldela behörigheter**</span><span class="sxs-lookup"><span data-stu-id="cf280-107">**Assign Permissions**</span></span>

<span data-ttu-id="cf280-108">Om användaren har tilldelats en SharePoint-licens och fortfarande får ett meddelande om nekad åtkomst, kontrollera att de har [rätt behörighetsnivå](https://docs.microsoft.com/sharepoint/understanding-permission-levels) tilldelad.</span><span class="sxs-lookup"><span data-stu-id="cf280-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="cf280-109">**Överväg att använda funktionen för åtkomstbegäran**</span><span class="sxs-lookup"><span data-stu-id="cf280-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="cf280-110">Med [funktionen för åtkomstbegäran](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) kan personer begära åtkomst till innehåll som de för närvarande inte har behörighet att se.</span><span class="sxs-lookup"><span data-stu-id="cf280-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="cf280-111">**Tillåt anpassade skript kan orsaka åtkomst nekad problem**</span><span class="sxs-lookup"><span data-stu-id="cf280-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="cf280-112">Det finns vissa scenarier där funktionen *Tillåt anpassade skript* kan utgöra en åtkomst nekad.</span><span class="sxs-lookup"><span data-stu-id="cf280-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="cf280-113">En lista över funktioner som berörs, säkerhetsöverväganden och möjligheten att inaktivera funktionen.</span><span class="sxs-lookup"><span data-stu-id="cf280-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="cf280-114">Besök [Tillåt eller förhindra anpassade skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="cf280-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

