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
# <a name="unable-to-delete-items"></a>Det gick inte att ta bort objekt

Bevarandeprinciper kan orsaka detta, måste du antingen inaktivera eller utesluta respektive spärr som orsakar problemet. När en bevarandeprincip eller spärr har tagits bort kan det ta upp till 24 timmar innan ändringen träder i kraft. Kontrollera att det inte finns en inställning för [bevarandeprincip](https://docs.microsoft.com/office365/securitycompliance/retention-policies) på objektet.

Platsen kan ha överskridit lagringsgränsen, öka [platskvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) och ta bort objektet.

Kontrollera att objektet inte [är utcheckat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) till en annan användare.

Slutligen kan administratörer använda [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som innehåller ett bibliotek med PowerShell-kommandon som gör att du kan utföra komplexa hanteringsåtgärder som tvinga bort envisa objekt.
- [Ta bort PNP-fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Ta bort PNP-mapp](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Ta bort PNP-listobjekt](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Ta bort PNP-lista](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Ta bort PNP-fält (kolumn)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)