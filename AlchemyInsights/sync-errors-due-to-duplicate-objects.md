---
title: 902 (Synkroniseringsfel på grund av dubblettobjekt)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767157"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="7353b-102">Synkroniseringsfel på grund av dubblettobjekt</span><span class="sxs-lookup"><span data-stu-id="7353b-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="7353b-103">Ett av följande felmeddelanden kan visas när katalogsynkroniseringen är klar i Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="7353b-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="7353b-104">Det går inte att uppdatera objektet i Microsoft Online Services eftersom följande attribut som är associerade med det här objektet har värden som kanske redan är associerade med ett annat objekt i den lokala katalogen.</span><span class="sxs-lookup"><span data-stu-id="7353b-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="7353b-105">Det finns redan ett synkroniserat objekt med samma proxyadress i microsoft onlinetjänstkatalogen.</span><span class="sxs-lookup"><span data-stu-id="7353b-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="7353b-106">Det går inte att uppdatera det här objektet eftersom följande attribut som är associerade med det här objektet har värden som kanske redan är associerade med ett annat objekt i dina lokala katalogtjänster: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="7353b-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="7353b-107">Om du vill identifiera och åtgärda problemet hämtar och kör [du IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="7353b-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="7353b-108">Mer information finns i [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="7353b-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
