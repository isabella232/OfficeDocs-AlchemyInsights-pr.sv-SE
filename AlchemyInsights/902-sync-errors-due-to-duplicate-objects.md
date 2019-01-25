---
title: 902 (synkroniseringsfel på Duplicera objekt)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492765"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="a15b5-102">Synkroniseringsfel på Duplicera objekt</span><span class="sxs-lookup"><span data-stu-id="a15b5-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="a15b5-103">Du kan få något av följande felmeddelanden visas när directory-synkroniseringen är klar:</span><span class="sxs-lookup"><span data-stu-id="a15b5-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="a15b5-104">Det gick inte att uppdatera det här objektet i Microsoft Online Services eftersom följande attribut som associeras med det här objektet har värden som redan kan vara kopplad till ett annat objekt i den lokala katalogen.</span><span class="sxs-lookup"><span data-stu-id="a15b5-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="a15b5-105">Det finns redan ett synkroniserat objekt med samma proxyadress i Microsoft Online Services-katalogen.</span><span class="sxs-lookup"><span data-stu-id="a15b5-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="a15b5-106">Det gick inte att uppdatera det här objektet eftersom följande attribut som associeras med det här objektet har värden som redan kan vara kopplad till ett annat objekt i din lokala katalogtjänster: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a15b5-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="a15b5-107">Hämta och kör [IdFix DirSync fel reparation verktyg](https://www.microsoft.com/download/details.aspx?id=36832)för att identifiera och åtgärda problemet.</span><span class="sxs-lookup"><span data-stu-id="a15b5-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="a15b5-108">Mer information finns i [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="a15b5-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

