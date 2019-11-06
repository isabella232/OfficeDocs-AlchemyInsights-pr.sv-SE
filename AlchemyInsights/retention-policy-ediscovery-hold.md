---
title: 2609-bevarande-eller-eDiscovery-håll
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994100"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="9c3c0-102">Det går inte att ta bort objekt i SharePoint Online eller OneDrive för företag</span><span class="sxs-lookup"><span data-stu-id="9c3c0-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="9c3c0-103">Du eller dina användare kan inte ta bort objekt i SharePoint Online eller OneDrive för företag eftersom en bevarandeprincip, bevarande etikett eller e-informationsavslöjande håller tillämpas på en SharePoint-webbplats för OneDrive eller ett visst objekt.</span><span class="sxs-lookup"><span data-stu-id="9c3c0-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="9c3c0-104">Detta inkluderar att det inte går att ta bort ett dokument, en dokumentversion, en mapp, ett dokumentbibliotek, en lista, en app, en webbplats eller en webbplatssamling.</span><span class="sxs-lookup"><span data-stu-id="9c3c0-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="9c3c0-105">Här är några exempel på felmeddelanden som kan tas emot om du försöker ta bort ett objekt som behålls:</span><span class="sxs-lookup"><span data-stu-id="9c3c0-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="9c3c0-106">"Den här webbplatsen kan inte tas bort eftersom den ingår i en e-informationsavslöjande spärr eller bevarandeprincip"</span><span class="sxs-lookup"><span data-stu-id="9c3c0-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="9c3c0-107">"Den här webbplatsen har en efterlevnadsprincip inställd på att blockera borttagning"</span><span class="sxs-lookup"><span data-stu-id="9c3c0-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="9c3c0-108">"En efterlevnadsprincip blockerar för närvarande den här webbplats borttagningen"</span><span class="sxs-lookup"><span data-stu-id="9c3c0-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="9c3c0-109">"Den här webbplatssamlingen kan inte tas bort eftersom den innehåller webbplatser som ingår i en e-informationsavslöjande spärr eller bevarandeprincip"</span><span class="sxs-lookup"><span data-stu-id="9c3c0-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="9c3c0-110">"Du måste ta bort alla objekt i den här mappen innan du tar bort mappen"</span><span class="sxs-lookup"><span data-stu-id="9c3c0-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="9c3c0-111">"Versioner av det här objektet kan inte tas bort eftersom den är spärrad eller bevarandeprincip"</span><span class="sxs-lookup"><span data-stu-id="9c3c0-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="9c3c0-112">"Objektet kan inte raderas när det är spärrad"</span><span class="sxs-lookup"><span data-stu-id="9c3c0-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="9c3c0-113">"Etiketten som används för det här objektet förhindrar att redigeras eller tas bort"</span><span class="sxs-lookup"><span data-stu-id="9c3c0-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="9c3c0-114">"Listan kan inte tas bort när spärrad eller bevarandeprincip"</span><span class="sxs-lookup"><span data-stu-id="9c3c0-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="9c3c0-115">"Listan kan inte tas bort om den är blockerad eller om en bevarandeprincip tillämpas på den"</span><span class="sxs-lookup"><span data-stu-id="9c3c0-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="9c3c0-116">Om du vill ta bort objekt i något av dessa scenarier måste bevarandeprincip, bevarande etikett eller e-informationsavslöjande hålla tas bort (eller en webbplats måste undantas från en bevarandeprincip).</span><span class="sxs-lookup"><span data-stu-id="9c3c0-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="9c3c0-117">Du måste antingen inaktivera eller utesluta respektive spärr som orsakar problemet.</span><span class="sxs-lookup"><span data-stu-id="9c3c0-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="9c3c0-118">När en bevarandeprincip eller spärr tas bort kan det ta upp till 24 timmar innan ändringen träder i kraft.</span><span class="sxs-lookup"><span data-stu-id="9c3c0-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="9c3c0-119">Information om de olika bevarande-och spärrfunktioner som kan tillämpas på SharePoint-webbplatser och OneDrive-konton finns i något av följande avsnitt.</span><span class="sxs-lookup"><span data-stu-id="9c3c0-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="9c3c0-120">Översikt över bevarandeprinciper</span><span class="sxs-lookup"><span data-stu-id="9c3c0-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="9c3c0-121">Översikt över bevarande etiketter</span><span class="sxs-lookup"><span data-stu-id="9c3c0-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="9c3c0-122">Hantera spärrar i Avancerad eDiscovery</span><span class="sxs-lookup"><span data-stu-id="9c3c0-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="9c3c0-123">eDiscovery innehar</span><span class="sxs-lookup"><span data-stu-id="9c3c0-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="9c3c0-124">Policyer för äldre webbplats stängning och borttagning</span><span class="sxs-lookup"><span data-stu-id="9c3c0-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
