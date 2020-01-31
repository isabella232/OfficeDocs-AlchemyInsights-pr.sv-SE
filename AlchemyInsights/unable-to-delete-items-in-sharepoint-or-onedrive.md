---
title: Det gick inte att ta bort objekt i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571289"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="ac1f2-102">Det gick inte att ta bort objekt</span><span class="sxs-lookup"><span data-stu-id="ac1f2-102">Unable to delete items</span></span>

<span data-ttu-id="ac1f2-103">Bevarandeprinciper kan orsaka detta, måste du antingen inaktivera eller utesluta respektive spärr som orsakar problemet.</span><span class="sxs-lookup"><span data-stu-id="ac1f2-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="ac1f2-104">När en bevarandeprincip eller spärr har tagits bort kan det ta upp till 24 timmar innan ändringen träder i kraft.</span><span class="sxs-lookup"><span data-stu-id="ac1f2-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="ac1f2-105">Kontrollera att det inte finns en inställning för [bevarandeprincip](https://docs.microsoft.com/office365/securitycompliance/retention-policies) på objektet.</span><span class="sxs-lookup"><span data-stu-id="ac1f2-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="ac1f2-106">Platsen kan ha överskridit lagringsgränsen, öka [platskvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) och ta bort objektet.</span><span class="sxs-lookup"><span data-stu-id="ac1f2-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="ac1f2-107">Kontrollera att objektet inte [är utcheckat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) till en annan användare.</span><span class="sxs-lookup"><span data-stu-id="ac1f2-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="ac1f2-108">Slutligen kan administratörer använda [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som innehåller ett bibliotek med PowerShell-kommandon som gör att du kan utföra komplexa hanteringsåtgärder som tvinga bort envisa objekt.</span><span class="sxs-lookup"><span data-stu-id="ac1f2-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="ac1f2-109">Ta bort PNP-fil</span><span class="sxs-lookup"><span data-stu-id="ac1f2-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="ac1f2-110">Ta bort PNP-mapp</span><span class="sxs-lookup"><span data-stu-id="ac1f2-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="ac1f2-111">Ta bort PNP-listobjekt</span><span class="sxs-lookup"><span data-stu-id="ac1f2-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="ac1f2-112">Ta bort PNP-lista</span><span class="sxs-lookup"><span data-stu-id="ac1f2-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="ac1f2-113">Ta bort PNP-fält (kolumn)</span><span class="sxs-lookup"><span data-stu-id="ac1f2-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)