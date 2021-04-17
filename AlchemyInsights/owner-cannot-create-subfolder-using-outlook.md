---
title: Det går inte att skapa en undermapp i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836153"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="b098a-102">Det går inte att skapa en undermapp i Outlook</span><span class="sxs-lookup"><span data-stu-id="b098a-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="b098a-103">**Det finns ett pågående problem med att ägare av gemensamma mappar skapar undermappar med Outlook. Problemet kommer att åtgärdas inom kort.**</span><span class="sxs-lookup"><span data-stu-id="b098a-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="b098a-104">Under tiden kan du använda någon av följande lösningar:</span><span class="sxs-lookup"><span data-stu-id="b098a-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="b098a-105">Använd Outlook för MAC för att skapa undermappen eftersom problemet bara påverkar Outlook för skrivbordsfönster (alla versioner)</span><span class="sxs-lookup"><span data-stu-id="b098a-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="b098a-106">Be administratören skapa undermappen med EXO Shell eller EAC</span><span class="sxs-lookup"><span data-stu-id="b098a-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="b098a-107">Ändra rutan DefaultPublicFolderMailbox/EffectivePublicFolderMailbox för användaren till en annan postlåda än innehållspostlådan för mappen som orsakar problemet</span><span class="sxs-lookup"><span data-stu-id="b098a-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="b098a-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="b098a-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="b098a-109">Vänta en timme, starta om Outlook-klienten</span><span class="sxs-lookup"><span data-stu-id="b098a-109">Wait for an hour, restart outlook client</span></span>