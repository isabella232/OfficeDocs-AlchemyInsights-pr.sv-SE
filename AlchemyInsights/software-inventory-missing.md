---
title: Programvaruinventering saknas eller är felaktig
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676516"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="e1e28-102">Programvaruinventering saknas eller är felaktig</span><span class="sxs-lookup"><span data-stu-id="e1e28-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="e1e28-103">Software Inventory in Hantering av hot och säkerhetsrisker (TVM) är en lista över kända program i din organisation med officiella gemensam plattform uppräkning (CPE).</span><span class="sxs-lookup"><span data-stu-id="e1e28-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="e1e28-104">Eventuella svagheter publiceras inte för programvaruprodukter utan ett officiellt CPE.</span><span class="sxs-lookup"><span data-stu-id="e1e28-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="e1e28-105">Inventeringen omfattar även information som namnet på leverantören, antal svagheter, hot och antal exponerade enheter.</span><span class="sxs-lookup"><span data-stu-id="e1e28-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="e1e28-106">Programvaruändringar på enheter återspeglas vanligtvis i säkerhetsportaler inom två timmar.</span><span class="sxs-lookup"><span data-stu-id="e1e28-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="e1e28-107">Ibland kan det dock ta längre tid.</span><span class="sxs-lookup"><span data-stu-id="e1e28-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="e1e28-108">Det finns för närvarande inget sätt att tvinga fram synkronisering. det här är en kontinuerlig bedömning.</span><span class="sxs-lookup"><span data-stu-id="e1e28-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="e1e28-109">Om du har gjort en ändring av programvaran och ändringen inte återspeglas korrekt i TVM efter 5 timmar gör du så här:</span><span class="sxs-lookup"><span data-stu-id="e1e28-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="e1e28-110">Kontrollera avsnittet med programvarubevis för att förstå hur programvaran identifierades.</span><span class="sxs-lookup"><span data-stu-id="e1e28-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="e1e28-111">Kontrollera att programvaran stöds.</span><span class="sxs-lookup"><span data-stu-id="e1e28-111">Make sure that the software is supported.</span></span> <span data-ttu-id="e1e28-112">Programvaran kan bara visas på enhetsnivå även om den för närvarande inte stöds av Hantering av hot och säkerhetsrisker.</span><span class="sxs-lookup"><span data-stu-id="e1e28-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="e1e28-113">Men endast begränsade data finns tillgängliga.</span><span class="sxs-lookup"><span data-stu-id="e1e28-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="e1e28-114">Information om hur du rapporterar felaktigheter från portalen finns i [Rapportens felaktigheter.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="e1e28-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="e1e28-115">**Obs!** Att rapportera fel från MDE-portalen är en envägskanal för teknik.</span><span class="sxs-lookup"><span data-stu-id="e1e28-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="e1e28-116">Om problemet är brådskande ska du öppna ett support ärende.</span><span class="sxs-lookup"><span data-stu-id="e1e28-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="e1e28-117">Mer information finns i Lager [av programvara - Hantering av hot och säkerhetsrisker](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="e1e28-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>