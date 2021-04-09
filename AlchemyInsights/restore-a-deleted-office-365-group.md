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
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="5b82f-102">Återställa en borttagna Microsoft 365-grupp</span><span class="sxs-lookup"><span data-stu-id="5b82f-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="5b82f-103">Du kan återställa en borttagen Microsoft 365-grupp eller Microsoft Teams inom 30 dagar från borttagningen.</span><span class="sxs-lookup"><span data-stu-id="5b82f-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="5b82f-104">Gå till [administrationscentret för Microsoft 365](https://aka.ms/RestoreDeletedGroup) för att logga in på en lista över de borttagna grupperna och teamen.</span><span class="sxs-lookup"><span data-stu-id="5b82f-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="5b82f-105">**Obs!** Logga in med det konto som har tilldelats till antingen innehavaradministratören eller gruppadministratörsrollen.</span><span class="sxs-lookup"><span data-stu-id="5b82f-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="5b82f-106">Välj den borttagna Microsoft 365-gruppen/Teams som ska återställas och klicka på **återställ grupp**.</span><span class="sxs-lookup"><span data-stu-id="5b82f-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="5b82f-107">Om gruppen inte kan återställas på grund av en SMTP-adress i konflikt kan du använda följande kommando för att hitta det objekt som orsakar konflikter och ta bort SMTP-adressen:</span><span class="sxs-lookup"><span data-stu-id="5b82f-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="5b82f-108">**Obs!** I vissa fall kan det ta upp till ett dygn för gruppen och alla data att återställas.</span><span class="sxs-lookup"><span data-stu-id="5b82f-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="5b82f-109">Mer information och hur du återställer grupper med hjälp av PowerShell finns i [Återställa en borttagna Microsoft 365-grupp.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="5b82f-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>