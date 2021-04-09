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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645149"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Återställa en borttagna Microsoft 365-grupp

Du kan återställa en borttagen Microsoft 365-grupp eller Microsoft Teams inom 30 dagar från borttagningen.

1. Gå till [administrationscentret för Microsoft 365](https://aka.ms/RestoreDeletedGroup) för att logga in på en lista över de borttagna grupperna och teamen.

    **Obs!** Logga in med det konto som har tilldelats till antingen innehavaradministratören eller gruppadministratörsrollen.

1. Välj den borttagna Microsoft 365-gruppen/Teams som ska återställas och klicka på **återställ grupp**.

    Om gruppen inte kan återställas på grund av en SMTP-adress i konflikt kan du använda följande kommando för att hitta det objekt som orsakar konflikter och ta bort SMTP-adressen:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Obs!** I vissa fall kan det ta upp till ett dygn för gruppen och alla data att återställas.

    Mer information och hur du återställer grupper med hjälp av PowerShell finns i [Återställa en borttagna Microsoft 365-grupp.](https://go.microsoft.com/fwlink/?linkid=867802)