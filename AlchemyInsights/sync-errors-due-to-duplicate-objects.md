---
title: 902 (synkroniseringsfel på Duplicera objekt)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420936"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="75cee-102">Synkroniseringsfel på Duplicera objekt</span><span class="sxs-lookup"><span data-stu-id="75cee-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="75cee-103">Du kan få något av följande felmeddelanden visas när directory-synkroniseringen är klar:</span><span class="sxs-lookup"><span data-stu-id="75cee-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>

- <span data-ttu-id="75cee-104">Det gick inte att uppdatera det här objektet i Microsoft Online Services eftersom följande attribut som associeras med det här objektet har värden som redan kan vara kopplad till ett annat objekt i den lokala katalogen.</span><span class="sxs-lookup"><span data-stu-id="75cee-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="75cee-105">Det finns redan ett synkroniserat objekt med samma proxyadress i Microsoft Online Services-katalogen.</span><span class="sxs-lookup"><span data-stu-id="75cee-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="75cee-106">Det gick inte att uppdatera det här objektet eftersom följande attribut som associeras med det här objektet har värden som redan kan vara kopplad till ett annat objekt i din lokala katalogtjänster: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="75cee-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="75cee-107">Hämta och kör [IdFix DirSync fel reparation verktyg](https://www.microsoft.com/download/details.aspx?id=36832)för att identifiera och åtgärda problemet.</span><span class="sxs-lookup"><span data-stu-id="75cee-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="75cee-108">Mer information finns i [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="75cee-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
