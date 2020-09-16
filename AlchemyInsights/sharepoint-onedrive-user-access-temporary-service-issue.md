---
title: Prestanda problem-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771262"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="d8126-102">SharePoint eller OneDrive långsamt, otillgängligt eller inte tillgängligt för flera användare</span><span class="sxs-lookup"><span data-stu-id="d8126-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="d8126-103">Om en OneDrive-eller SharePoint-webbplats inte är tillgänglig för flera användare som tidigare hade åtkomst kan det finnas ett tillfälligt tjänst problem.</span><span class="sxs-lookup"><span data-stu-id="d8126-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="d8126-104">[Kontrol lera instrument panelen för tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="d8126-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="d8126-105">**Lägga till och licensiera användaren**</span><span class="sxs-lookup"><span data-stu-id="d8126-105">**Add and license the user**</span></span>

<span data-ttu-id="d8126-106">Se till att [tilldela licenser till användare i Microsoft 365 för företag](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="d8126-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="d8126-107">**Tilldela behörigheter**</span><span class="sxs-lookup"><span data-stu-id="d8126-107">**Assign Permissions**</span></span>

<span data-ttu-id="d8126-108">Om användaren har tilldelats en SharePoint-licens och fortfarande får ett meddelande om nekad åtkomst bör du kontrol lera att de har [rätt behörighets nivå](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="d8126-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="d8126-109">**Överväg att använda funktionen för åtkomstbegäran**</span><span class="sxs-lookup"><span data-stu-id="d8126-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="d8126-110">Med [funktionen](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) åtkomstbegäran kan användarna begära åtkomst till innehåll som de inte har behörighet att se.</span><span class="sxs-lookup"><span data-stu-id="d8126-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="d8126-111">**Tillåt anpassat skript kan orsaka problem med åtkomst nekande**</span><span class="sxs-lookup"><span data-stu-id="d8126-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="d8126-112">Det finns vissa scenarier där funktionen för *att tillåta anpassade skript* kan visa upp en åtkomst nekad.</span><span class="sxs-lookup"><span data-stu-id="d8126-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="d8126-113">En lista över de funktioner som påverkas finns i säkerhets aspekter och möjligheten att inaktivera funktionen.</span><span class="sxs-lookup"><span data-stu-id="d8126-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="d8126-114">Gå till [Tillåt eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="d8126-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

