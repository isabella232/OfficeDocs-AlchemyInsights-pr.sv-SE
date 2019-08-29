---
title: Återställa borttagna postlåda
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 44b23be5e75a0669821bbeb07b0f064eeef6d021
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666390"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="d2310-102">Återställa en borttagen postlåda</span><span class="sxs-lookup"><span data-stu-id="d2310-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="d2310-103">När en användare förlorar en Exchange Online-licens, deras postlåda finns kvar i 30 dagar och kan återställas genom att helt enkelt tilldela licensen för användaren.</span><span class="sxs-lookup"><span data-stu-id="d2310-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="d2310-104">*Detta fungerar bara inom 30 dagar.*</span><span class="sxs-lookup"><span data-stu-id="d2310-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="d2310-105">Gå till **användare** i Microsoft 365 administratörscenter, \> sidan **aktiv användare** .</span><span class="sxs-lookup"><span data-stu-id="d2310-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="d2310-106">Markera användaren i fråga.</span><span class="sxs-lookup"><span data-stu-id="d2310-106">Select the user in question.</span></span>

2. <span data-ttu-id="d2310-107">Tilldela Exchange Online-licens och välj **Spara ändringar**på fliken **licenser och appar** .</span><span class="sxs-lookup"><span data-stu-id="d2310-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="d2310-108">Om du försöker återställa en delad postlåda är också återvinningsbara i 30 dagar.</span><span class="sxs-lookup"><span data-stu-id="d2310-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="d2310-109">Du hittar dem under **användare** \> **borttagna användare**. delade postlådor kräver inte en licens.</span><span class="sxs-lookup"><span data-stu-id="d2310-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="d2310-110">Om du upptäcker att du behöver återställa en borttagen användare, finns i [återställa en användare i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="d2310-110">If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  