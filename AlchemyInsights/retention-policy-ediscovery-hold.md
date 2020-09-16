---
title: 2609-bevarande-eller-eDiscovery-spärr
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: dee208560e7576597e20aec897f42432d7973727
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727909"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="5f96a-102">Det går inte att ta bort objekt i SharePoint Online eller OneDrive för företag</span><span class="sxs-lookup"><span data-stu-id="5f96a-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="5f96a-103">Du eller användarna kan kanske inte ta bort objekt i SharePoint Online eller OneDrive för företag eftersom en bevarande princip, bevarande etikett eller eDiscovery-undantag används på en SharePoint-webbplats för OneDrive eller till ett specifikt objekt.</span><span class="sxs-lookup"><span data-stu-id="5f96a-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="5f96a-104">Det här inkluderar inte att ta bort ett dokument, en dokument version, en mapp, ett dokument bibliotek, en lista, en app, en webbplats eller en webbplats samling.</span><span class="sxs-lookup"><span data-stu-id="5f96a-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> 

<span data-ttu-id="5f96a-105">Om du vill ta bort objekt i något av dessa scenario måste bevarande princip, bevarande etikett eller eDiscovery-undantag tas bort (eller en webbplats måste undantas från en bevarande princip).</span><span class="sxs-lookup"><span data-stu-id="5f96a-105">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="5f96a-106">Du måste antingen inaktivera eller exkludera respektive undantag som orsakar problemet.</span><span class="sxs-lookup"><span data-stu-id="5f96a-106">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="5f96a-107">När en bevarande princip eller undantag har tagits bort kan det ta upp till 24 timmar innan ändringen börjar gälla.</span><span class="sxs-lookup"><span data-stu-id="5f96a-107">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="5f96a-108">Information om de olika funktionerna för bevarande och lagring som kan tillämpas på SharePoint-webbplatser och OneDrive-konton finns i följande avsnitt.</span><span class="sxs-lookup"><span data-stu-id="5f96a-108">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="5f96a-109">Översikt över bevarande principer</span><span class="sxs-lookup"><span data-stu-id="5f96a-109">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [<span data-ttu-id="5f96a-110">Översikt över bevarande etiketter</span><span class="sxs-lookup"><span data-stu-id="5f96a-110">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [<span data-ttu-id="5f96a-111">Hantera undantag i Avancerad eDiscovery</span><span class="sxs-lookup"><span data-stu-id="5f96a-111">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [<span data-ttu-id="5f96a-112">eDiscovery-undantag</span><span class="sxs-lookup"><span data-stu-id="5f96a-112">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [<span data-ttu-id="5f96a-113">Avsluts och borttagnings principer för äldre webbplatser</span><span class="sxs-lookup"><span data-stu-id="5f96a-113">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)