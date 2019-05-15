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
# <a name="unable-to-delete-items"></a>Det går inte att ta bort objekt

Har du problem att ta bort objekt?

- Kontrollera alltid att du har [behörighet](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) att ta bort objektet eller en [administratör för webbplatssamlingen](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) försök ta bort objektet.

- Se till att det inte är en [bevarandeprincip](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) inställning på objektet.

- Kontrollera att objektet inte är [utcheckad](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) till en annan användare.

- Slutligen kan administratörer använda [SharePoint mönster och praxis](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som innehåller ett bibliotek med PowerShell-kommandon som du kan utföra hanteringsåtgärder för komplexa som tvingar stubborn objekt tas bort. 
- [Ta bort PNP-fil](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Ta bort PNP-mappen](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Ta bort PNP listobjekt](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Ta bort PNP lista](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Ta bort PNP fält (kolumn)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)