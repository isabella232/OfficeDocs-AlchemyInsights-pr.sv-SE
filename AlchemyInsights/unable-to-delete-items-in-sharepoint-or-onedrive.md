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
# <a name="unable-to-delete-items"></a>Det går inte att ta bort objekt

Bevarandeprinciper kan orsaka detta, du måste antingen inaktivera eller utesluta respektive spärr som orsakar det här problemet. När en bevarandeprincip eller spärr har tagits bort kan det ta upp till 24 timmar innan ändringen börjar gälla. Kontrollera att det inte finns någon [bevarandeprincipinställning](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) för artikeln.

Platsen kan ha överskridit lagringsgränsen, ökat [platskvoten](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) och tagit bort objektet.

Kontrollera att objektet inte är [utcheckat](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) till en annan användare.

Slutligen kan administratörer använda [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) som innehåller ett bibliotek med PowerShell-kommandon som gör att du kan utföra komplexa hanteringsåtgärder som att tvinga bort envisa objekt.
- [Ta bort PNP-fil](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Ta bort PNP-mapp](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Ta bort PNP-listobjekt](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Ta bort PNP-lista](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Ta bort PNP-fält (kolumn)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)