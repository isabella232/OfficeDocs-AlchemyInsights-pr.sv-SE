---
title: Ägaren kan inte skapa undermapp med Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749146"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="cb261-102">Ägaren kan inte skapa undermapp med Outlook</span><span class="sxs-lookup"><span data-stu-id="cb261-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="cb261-103">**Det finns ett pågående problem med att ägare av gemensamma mappar skapar undermappar med Outlook. Problemet kommer att åtgärdas snart.**</span><span class="sxs-lookup"><span data-stu-id="cb261-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="cb261-104">Under tiden använder du någon av följande lösningar:</span><span class="sxs-lookup"><span data-stu-id="cb261-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="cb261-105">Använd Outlook för MAC för att skapa undermappen eftersom problemet endast påverkar Outlook för skrivbordsfönster (alla versioner)</span><span class="sxs-lookup"><span data-stu-id="cb261-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="cb261-106">Låt administratören skapa undermappen med EXO Shell eller EAC</span><span class="sxs-lookup"><span data-stu-id="cb261-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="cb261-107">Ändra DefaultPublicFolderMailbox/EffectivePublicFolderMailbox på användaren till annan postlåda än innehållspostlådan för mappen som orsakar problem</span><span class="sxs-lookup"><span data-stu-id="cb261-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="cb261-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="cb261-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="cb261-109">Vänta i en timme, starta om Outlook-klienten</span><span class="sxs-lookup"><span data-stu-id="cb261-109">Wait for an hour, restart outlook client</span></span>