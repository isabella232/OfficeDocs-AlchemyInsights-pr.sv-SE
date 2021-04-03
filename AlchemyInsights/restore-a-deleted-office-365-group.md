---
title: Återställa en borttagna Microsoft 365-grupp
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505728"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Återställa en borttagna Microsoft 365-grupp

Du kan återställa en borttagen Microsoft 365-grupp eller Microsoft Teams inom 30 dagar från borttagningen.

1. Om du vill logga in på administrationscentret för Microsoft 365 och visa en lista över borttagna grupper och team går du till administrationscentret för [Microsoft 365.](https://aka.ms/RestoreDeletedGroup)

    **Obs!** Logga in med det konto som har tilldelats till antingen innehavaradministratören eller gruppadministratörsrollen.

1. Välj den borttagna Microsoft 365-gruppen/Teams som ska återställas och klicka på **återställ grupp**.

    Om gruppen inte kan återställas på grund av en SMTP-adress i konflikt kan du använda följande kommando för att hitta det objekt som orsakar konflikter och ta bort SMTP-adressen:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Obs!** I vissa fall kan det ta upp till ett dygn för gruppen och alla data att återställas.

    Mer information och hur du återställer grupper med hjälp av PowerShell finns i [Återställa en borttagna Microsoft 365-grupp.](https://go.microsoft.com/fwlink/?linkid=867802)