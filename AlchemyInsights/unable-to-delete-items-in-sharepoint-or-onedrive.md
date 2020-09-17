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
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806129"
---
# <a name="unable-to-delete-items"></a>Det går inte att ta bort objekt

Bevarande principer kan orsaka detta, men du måste antingen inaktivera eller exkludera respektive undantag som orsakar problemet. När en bevarande princip eller undantag har tagits bort kan det ta upp till 24 timmar innan ändringen börjar gälla. Kontrol lera att det inte finns någon [bevarande princip](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) inställning för objektet.

Webbplatsen kan ha överskridit lagrings gränsen, öka [kvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) och ta bort objektet.

Se till att objektet inte är [utcheckat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) till en annan användare.

Slutligen kan administratörer använda [SharePoint-mönster och-praxis](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) som innehåller ett bibliotek med PowerShell-kommandon som gör det möjligt att utföra komplexa hanterings åtgärder, till exempel att tvinga bort Stubborn-objekt.
- [Ta bort PNP-fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Ta bort PNP-mapp](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Ta bort PNP-listobjekt](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Ta bort PNP-lista](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Ta bort PNP-fält (kolumn)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)