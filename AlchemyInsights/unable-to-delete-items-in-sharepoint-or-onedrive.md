---
title: Det går inte att ta bort objekt i SharePoint eller OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748594"
---
# <a name="unable-to-delete-items"></a>Det går inte att ta bort objekt

Har du problem med att ta bort SharePoint-objekt?

- Kontrollera alltid att du har [rätt behörighet](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) för att ta bort objektet eller låta en [webbplatssamlingsadministratör](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) försöka ta bort objektet.

- Kontrollera att det inte finns en inställning för [bevarandeprincip](https://docs.microsoft.com/office365/securitycompliance/retention-policies) för objektet.

- Kontrollera att objektet inte är [utcheckat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) till en annan användare.

- Slutligen kan administratörer använda [SharePoint-mönster och-metoder](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) som innehåller ett bibliotek med PowerShell-kommandon som gör det möjligt att utföra komplexa hanteringsåtgärder, till exempel framtvinga borttagning av envisa objekt.
- [Ta bort PNP-fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Ta bort PNP-mapp](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Ta bort PNP-listobjekt](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Ta bort PNP-lista](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Ta bort PNP-fält (kolumn)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)