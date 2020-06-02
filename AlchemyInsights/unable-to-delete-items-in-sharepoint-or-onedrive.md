---
title: Det går inte att ta bort objekt i SharePoint eller OneDrive
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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511994"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="73c83-102">Det går inte att ta bort objekt</span><span class="sxs-lookup"><span data-stu-id="73c83-102">Unable to delete items</span></span>

<span data-ttu-id="73c83-103">Bevarandeprinciper kan orsaka detta, du måste antingen inaktivera eller utesluta respektive spärr som orsakar det här problemet.</span><span class="sxs-lookup"><span data-stu-id="73c83-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="73c83-104">När en bevarandeprincip eller spärr har tagits bort kan det ta upp till 24 timmar innan ändringen börjar gälla.</span><span class="sxs-lookup"><span data-stu-id="73c83-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="73c83-105">Kontrollera att det inte finns någon [bevarandeprincipinställning](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) för artikeln.</span><span class="sxs-lookup"><span data-stu-id="73c83-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="73c83-106">Platsen kan ha överskridit lagringsgränsen, ökat [platskvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) och tagit bort objektet.</span><span class="sxs-lookup"><span data-stu-id="73c83-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="73c83-107">Kontrollera att objektet inte är [utcheckat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) till en annan användare.</span><span class="sxs-lookup"><span data-stu-id="73c83-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="73c83-108">Slutligen kan administratörer använda [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som innehåller ett bibliotek med PowerShell-kommandon som gör att du kan utföra komplexa hanteringsåtgärder som att tvinga bort envisa objekt.</span><span class="sxs-lookup"><span data-stu-id="73c83-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="73c83-109">Ta bort PNP-fil</span><span class="sxs-lookup"><span data-stu-id="73c83-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="73c83-110">Ta bort PNP-mapp</span><span class="sxs-lookup"><span data-stu-id="73c83-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="73c83-111">Ta bort PNP-listobjekt</span><span class="sxs-lookup"><span data-stu-id="73c83-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="73c83-112">Ta bort PNP-lista</span><span class="sxs-lookup"><span data-stu-id="73c83-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="73c83-113">Ta bort PNP-fält (kolumn)</span><span class="sxs-lookup"><span data-stu-id="73c83-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)