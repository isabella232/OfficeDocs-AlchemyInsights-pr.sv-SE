---
title: Det går inte att ta bort objekt i SharePoint eller OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057784"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="fc234-102">Det går inte att ta bort objekt</span><span class="sxs-lookup"><span data-stu-id="fc234-102">Unable to delete items</span></span>

<span data-ttu-id="fc234-103">Har du problem att ta bort objekt?</span><span class="sxs-lookup"><span data-stu-id="fc234-103">Having issues deleting items?</span></span>

- <span data-ttu-id="fc234-104">Kontrollera alltid att du har [behörighet](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) att ta bort objektet eller en [administratör för webbplatssamlingen](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) försök ta bort objektet.</span><span class="sxs-lookup"><span data-stu-id="fc234-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="fc234-105">Se till att det inte är en [bevarandeprincip](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) inställning på objektet.</span><span class="sxs-lookup"><span data-stu-id="fc234-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="fc234-106">Kontrollera att objektet inte är [utcheckad](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) till en annan användare.</span><span class="sxs-lookup"><span data-stu-id="fc234-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="fc234-107">Slutligen kan administratörer använda [SharePoint mönster och praxis](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som innehåller ett bibliotek med PowerShell-kommandon som du kan utföra hanteringsåtgärder för komplexa som tvingar stubborn objekt tas bort.</span><span class="sxs-lookup"><span data-stu-id="fc234-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="fc234-108">Ta bort PNP-fil</span><span class="sxs-lookup"><span data-stu-id="fc234-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="fc234-109">Ta bort PNP-mappen</span><span class="sxs-lookup"><span data-stu-id="fc234-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="fc234-110">Ta bort PNP listobjekt</span><span class="sxs-lookup"><span data-stu-id="fc234-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="fc234-111">Ta bort PNP lista</span><span class="sxs-lookup"><span data-stu-id="fc234-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="fc234-112">Ta bort PNP fält (kolumn)</span><span class="sxs-lookup"><span data-stu-id="fc234-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)