---
title: Det går inte att ta bort objekt i SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019601"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="abd68-102">Det går inte att ta bort objekt</span><span class="sxs-lookup"><span data-stu-id="abd68-102">Unable to delete items</span></span>

- <span data-ttu-id="abd68-103">Bevarande principer kan orsaka detta, men du måste antingen inaktivera eller exkludera respektive undantag som orsakar problemet.</span><span class="sxs-lookup"><span data-stu-id="abd68-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="abd68-104">När en bevarande princip eller undantag har tagits bort kan det ta upp till 24 timmar innan ändringen börjar gälla.</span><span class="sxs-lookup"><span data-stu-id="abd68-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="abd68-105">Kontrol lera att det inte finns någon [bevarande princip](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) inställning för objektet.</span><span class="sxs-lookup"><span data-stu-id="abd68-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="abd68-106">Webbplatsen kan ha överskridit lagrings gränsen, öka [kvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) och ta bort objektet.</span><span class="sxs-lookup"><span data-stu-id="abd68-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="abd68-107">Se till att objektet inte är [utcheckat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) till en annan användare.</span><span class="sxs-lookup"><span data-stu-id="abd68-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="abd68-108">Slutligen kan administratörer använda [SharePoint-mönster och-praxis](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) som innehåller ett bibliotek med PowerShell-kommandon som gör det möjligt att utföra komplexa hanterings åtgärder, till exempel att tvinga bort Stubborn-objekt.</span><span class="sxs-lookup"><span data-stu-id="abd68-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="abd68-109">Ta bort PNP-fil</span><span class="sxs-lookup"><span data-stu-id="abd68-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="abd68-110">Ta bort PNP-mapp</span><span class="sxs-lookup"><span data-stu-id="abd68-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="abd68-111">Ta bort PNP-listobjekt</span><span class="sxs-lookup"><span data-stu-id="abd68-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="abd68-112">Ta bort PNP-lista</span><span class="sxs-lookup"><span data-stu-id="abd68-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="abd68-113">Ta bort PNP-fält (kolumn)</span><span class="sxs-lookup"><span data-stu-id="abd68-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)