---
title: Ägaren kan inte skapa undermappen med Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665736"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="e58f7-102">Ägaren kan inte skapa undermappen med Outlook</span><span class="sxs-lookup"><span data-stu-id="e58f7-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="e58f7-103">**Det finns ett pågående problem med privata ägarnoder som skapar undermappar med Outlook. Problemet åtgärdas snart.**</span><span class="sxs-lookup"><span data-stu-id="e58f7-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="e58f7-104">Under tiden kan du använda någon av följande lösningar:</span><span class="sxs-lookup"><span data-stu-id="e58f7-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="e58f7-105">Använda Outlook för MAC för att skapa undermappen eftersom problemet endast påverkar Outlook för Skriv bords fönster (alla versioner)</span><span class="sxs-lookup"><span data-stu-id="e58f7-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="e58f7-106">Be administratören skapa undermappen med EXO skal eller UK</span><span class="sxs-lookup"><span data-stu-id="e58f7-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="e58f7-107">Ändra DefaultPublicFolderMailbox/EffectivePublicFolderMailbox för användaren till en annan post låda än innehålls post lådan för mappen som orsakar problemet</span><span class="sxs-lookup"><span data-stu-id="e58f7-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="e58f7-108">*Set-post låda Användare1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="e58f7-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="e58f7-109">Vänta i en timme, starta om Outlook-klient</span><span class="sxs-lookup"><span data-stu-id="e58f7-109">Wait for an hour, restart outlook client</span></span>