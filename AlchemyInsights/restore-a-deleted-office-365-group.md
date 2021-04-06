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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597461"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="412d3-102">Återställa en borttagna Microsoft 365-grupp</span><span class="sxs-lookup"><span data-stu-id="412d3-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="412d3-103">Du kan återställa en borttagen Microsoft 365-grupp eller Microsoft Teams inom 30 dagar från borttagningen.</span><span class="sxs-lookup"><span data-stu-id="412d3-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="412d3-104">Gå till [administrationscentret för Microsoft 365 för](https://aka.ms/RestoreDeletedGroup) att logga in och lista de borttagna grupperna och teamen.</span><span class="sxs-lookup"><span data-stu-id="412d3-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="412d3-105">**Obs!** Logga in med det konto som har tilldelats till antingen innehavaradministratören eller gruppadministratörsrollen.</span><span class="sxs-lookup"><span data-stu-id="412d3-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="412d3-106">Välj den borttagna Microsoft 365-gruppen/Teams som ska återställas och klicka på **återställ grupp**.</span><span class="sxs-lookup"><span data-stu-id="412d3-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="412d3-107">Om gruppen inte kan återställas på grund av en SMTP-adress i konflikt kan du använda följande kommando för att hitta det objekt som orsakar konflikter och ta bort SMTP-adressen:</span><span class="sxs-lookup"><span data-stu-id="412d3-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="412d3-108">**Obs!** I vissa fall kan det ta upp till ett dygn för gruppen och alla data att återställas.</span><span class="sxs-lookup"><span data-stu-id="412d3-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="412d3-109">Mer information och hur du återställer grupper med hjälp av PowerShell finns i [Återställa en borttagna Microsoft 365-grupp.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="412d3-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>