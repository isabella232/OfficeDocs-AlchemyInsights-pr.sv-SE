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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049535"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="99a2f-102">Det går inte att ta bort objekt</span><span class="sxs-lookup"><span data-stu-id="99a2f-102">Unable to delete items</span></span>

<span data-ttu-id="99a2f-103">Har du problem med att ta bort SharePoint-objekt?</span><span class="sxs-lookup"><span data-stu-id="99a2f-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="99a2f-104">Kontrollera alltid att du har [rätt behörighet](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) för att ta bort objektet eller låta en [webbplatssamlingsadministratör](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) försöka ta bort objektet.</span><span class="sxs-lookup"><span data-stu-id="99a2f-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="99a2f-105">Kontrollera att det inte finns en inställning för [bevarandeprincip](https://docs.microsoft.com/office365/securitycompliance/retention-policies) för objektet.</span><span class="sxs-lookup"><span data-stu-id="99a2f-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="99a2f-106">Kontrollera att objektet inte är [utcheckat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) till en annan användare.</span><span class="sxs-lookup"><span data-stu-id="99a2f-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="99a2f-107">Slutligen kan administratörer använda [SharePoint-mönster och-metoder](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) som innehåller ett bibliotek med PowerShell-kommandon som gör det möjligt att utföra komplexa hanteringsåtgärder, till exempel framtvinga borttagning av envisa objekt.</span><span class="sxs-lookup"><span data-stu-id="99a2f-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="99a2f-108">Ta bort PNP-fil</span><span class="sxs-lookup"><span data-stu-id="99a2f-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="99a2f-109">Ta bort PNP-mapp</span><span class="sxs-lookup"><span data-stu-id="99a2f-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="99a2f-110">Ta bort PNP-listobjekt</span><span class="sxs-lookup"><span data-stu-id="99a2f-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="99a2f-111">Ta bort PNP-lista</span><span class="sxs-lookup"><span data-stu-id="99a2f-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="99a2f-112">Ta bort PNP-fält (kolumn)</span><span class="sxs-lookup"><span data-stu-id="99a2f-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)